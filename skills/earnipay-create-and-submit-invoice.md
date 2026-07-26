---
name: Create and submit a FIRS-compliant invoice
description: Build an invoice from a customer and products, approve it, generate its IRN and QR code, and submit it to the tax authority via the Access Point Provider.
api: openapi/earnipay-e-invoicing-openapi-original.json
operations: [CustomerController_createCustomer_v1, ProductController_createProduct_v1, PaymentDetailController_create_v1, InvoiceController_validateInvoiceData_v1, InvoiceController_createInvoice_v1, InvoiceController_approveInvoice_v1, IrnGeneratorController_generateIRN_v1, InvoiceController_generateQrCode_v1, InvoiceController_submitToApp_v1, InvoiceController_downloadPdf_v1]
---

# Create and submit a FIRS-compliant invoice

Base URL: `https://e-invoicing.earnipay.com/v1`. Authenticate with the business JWT (or `X-API-Key` for a third-party integration). Complete the onboarding skill first.

1. **Ensure a customer exists** — `POST /v1/customers` (`CustomerController_createCustomer_v1`), or find one with `CustomerController_getCustomers_v1` (supports `?search=`). 409 = customer name already exists.
2. **Ensure products exist** — `POST /v1/products` (`ProductController_createProduct_v1`) with the correct tax category.
3. **Add payment details** — `POST /v1/payment-details` (`PaymentDetailController_create_v1`). Look up/verify bank accounts with `BankController_getBankList_v1` and `BankController_verifyBankAccount_v1`.
4. **Validate the draft** — `POST /v1/invoices/validate` (`InvoiceController_validateInvoiceData_v1`) before creating.
5. **Create the invoice** — `POST /v1/invoices` (`InvoiceController_createInvoice_v1`) referencing `customerId` and `paymentDetailId` plus line `items`.
6. **Approve it** — `POST /v1/invoices/{id}/approve` (`InvoiceController_approveInvoice_v1`) (or reject with `InvoiceController_rejectInvoice_v1`).
7. **Generate the IRN** — `POST /v1/irn-generator/generate` (`IrnGeneratorController_generateIRN_v1`).
8. **Generate the QR code** — `POST /v1/invoices/{id}/generate-qr` (`InvoiceController_generateQrCode_v1`).
9. **Submit to the tax authority** — `POST /v1/invoices/{id}/submit-to-app` (`InvoiceController_submitToApp_v1`).
10. **Download the PDF** — `GET /v1/invoices/{id}/pdf` (`InvoiceController_downloadPdf_v1`).

Rules: errors are standard JSON with 400/401/403/404/409 (see `errors/earnipay-problem-types.yml`); 404 on a bad `customerId`/`paymentDetailId`. No idempotency-key header — validate first, then create once.
