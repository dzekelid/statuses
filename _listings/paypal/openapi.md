swagger: "2.0"
x-collection-name: PayPal
x-complete: 1
info:
  title: PayPal (Sandbox)
  description: bring-payments-to-apps-mobile-and-social-with-adaptive-payments-bsandbox-api-b
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AdaptiveAccounts/GetVerifiedStatus:
    post:
      summary: Get Verified Status
      description: The GetVerifiedStatus API operation lets you check if a PayPal
        account status is verified. A PayPal account gains verified status under a
        variety of circumstances, such as when an account is linked to a verified
        funding source. Verified status serves to indicate a trust relationship. For
        more information about account verified status, refer to PayPal.com.
      operationId: AdaptiveAccounts.GetVerifiedStatus.post
      x-api-path-slug: adaptiveaccountsgetverifiedstatus-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Verified
      - Status
  /AdaptiveAccounts/SetFundingSourceConfirmed:
    post:
      summary: Set Funding Source Confirmed
      description: The SetFundingSourceConfirmed API operation lets your application
        set up bank accounts as funding sources for PayPal accounts.
      operationId: AdaptiveAccounts.SetFundingSourceConfirmed.post
      x-api-path-slug: adaptiveaccountssetfundingsourceconfirmed-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Verified
      - Status