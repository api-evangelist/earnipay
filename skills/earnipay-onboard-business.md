---
name: Onboard a business for FIRS e-invoicing
description: Register, verify, and configure an Earnipay business so it can submit FIRS-compliant invoices through an Access Point Provider.
api: openapi/earnipay-e-invoicing-openapi-original.json
operations: [AuthController_signup_v1, AuthController_verifyEmail_v1, AuthController_login_v1, BusinessController_createBusiness_v1, BusinessController_updateFirsConfig_v1, BusinessController_uploadCryptoKeys_v1, BusinessController_updateAppConfig_v1, BusinessController_testAppConnection_v1]
---

# Onboard a business for FIRS e-invoicing

Base URL: `https://e-invoicing.earnipay.com/v1`. Auth: obtain a JWT bearer token and send it as `Authorization: Bearer <token>`.

1. **Sign up** — `POST /v1/auth/signup` (`AuthController_signup_v1`) with the user's email and password.
2. **Verify email** — `POST /v1/auth/verify-email` (`AuthController_verifyEmail_v1`) with the emailed code. Resend with `AuthController_resendVerificationCode_v1` if it expired (400).
3. **Log in** — `POST /v1/auth/login` (`AuthController_login_v1`) to receive the JWT access token; refresh later with `AuthController_refreshToken_v1`.
4. **Create the business** — `POST /v1/businesses` (`BusinessController_createBusiness_v1`).
5. **Configure FIRS** — `PATCH /v1/businesses/{id}/firs-config` (`BusinessController_updateFirsConfig_v1`). Only the business OWNER may do this (else 403).
6. **Upload crypto keys** — `PATCH /v1/businesses/{id}/crypto-keys` (`BusinessController_uploadCryptoKeys_v1`).
7. **Configure the Access Point Provider** — `PATCH /v1/businesses/{id}/app-config` (`BusinessController_updateAppConfig_v1`).
8. **Test the connection** — `POST /v1/businesses/{id}/test-app-connection` (`BusinessController_testAppConnection_v1`) before going live.

Rules: 403 = insufficient role (many settings are OWNER-only); 409 = a business/TIN with that identity already exists. No idempotency-key contract — do not blindly retry create calls; re-read with `BusinessController_getUserBusinesses_v1` instead.
