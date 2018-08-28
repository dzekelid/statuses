---
name: Google Content API for Shopping
x-slug: google-content-api-for-shopping
description: 'API allowing retailers to manage their product feed content programmatically.
  Providing item-level data quality information: See if an item was disapproved because
  a landing page URL isn&rsquo;t working on a mobile device or if unique product identifiers
  are inaccurate. Faster pricing and availability updates: Ensure customers have the
  latest price-points and know what&rsquo;s in-stock before they click through to
  your site. More integration options: The newer API supports a broader choice of
  programming languages and data formats.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Statuses
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/apis.md
specificationVersion: "0.14"
apis:
- name: Content API for Shopping - Account Status Batch
  x-api-slug: accountstatusesbatch-post
  description: Retrieves account batch status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/accountstatusesbatch-post-openapi.md
- name: Content API for Shopping - Data Feed Status
  x-api-slug: datafeedstatusesbatch-post
  description: Retrieves data feed batch status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/datafeedstatusesbatch-post-openapi.md
- name: Content API for Shopping - Get Account Status
  x-api-slug: merchantidaccountstatuses-get
  description: Lists the statuses of the sub-accounts in your Merchant Center account.
    This method can only be called for multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidaccountstatuses-get-openapi.md
- name: Content API for Shopping - Get Account Status
  x-api-slug: merchantidaccountstatusesaccountid-get
  description: 'Retrieves the status of a Merchant Center account. This method can
    only be called for accounts to which the managing account has access: either the
    managing account itself or sub-accounts if the managing account is a multi-client
    account.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidaccountstatusesaccountid-get-openapi.md
- name: Content API for Shopping - Get Data Feed Status
  x-api-slug: merchantiddatafeedstatuses-get
  description: Lists the statuses of the datafeeds in your Merchant Center account.
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatuses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatuses-get-openapi.md
- name: Content API for Shopping - Get Data Feed Status
  x-api-slug: merchantiddatafeedstatusesdatafeedid-get
  description: Retrieves the status of a datafeed from your Merchant Center account.
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatusesdatafeedid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatusesdatafeedid-get-openapi.md
- name: Content API for Shopping - Get Product Status
  x-api-slug: merchantidproductstatuses-get
  description: Lists the statuses of the products in your Merchant Center account.
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidproductstatuses-get-openapi.md
- name: Content API for Shopping - Get Product Status
  x-api-slug: merchantidproductstatusesproductid-get
  description: Gets the status of a product from your Merchant Center account. This
    method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidproductstatusesproductid-get-openapi.md
- name: Content API for Shopping - Account Status Batch
  x-api-slug: accountstatusesbatch-post
  description: Retrieves account batch status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/accountstatusesbatch-post-openapi.md
- name: Content API for Shopping - Data Feed Status
  x-api-slug: datafeedstatusesbatch-post
  description: Retrieves data feed batch status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/datafeedstatusesbatch-post-openapi.md
- name: Content API for Shopping - Get Account Status
  x-api-slug: merchantidaccountstatuses-get
  description: Lists the statuses of the sub-accounts in your Merchant Center account.
    This method can only be called for multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidaccountstatuses-get-openapi.md
- name: Content API for Shopping - Get Account Status
  x-api-slug: merchantidaccountstatusesaccountid-get
  description: 'Retrieves the status of a Merchant Center account. This method can
    only be called for accounts to which the managing account has access: either the
    managing account itself or sub-accounts if the managing account is a multi-client
    account.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidaccountstatusesaccountid-get-openapi.md
- name: Content API for Shopping - Get Data Feed Status
  x-api-slug: merchantiddatafeedstatuses-get
  description: Lists the statuses of the datafeeds in your Merchant Center account.
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatuses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatuses-get-openapi.md
- name: Content API for Shopping - Get Data Feed Status
  x-api-slug: merchantiddatafeedstatusesdatafeedid-get
  description: Retrieves the status of a datafeed from your Merchant Center account.
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatusesdatafeedid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatusesdatafeedid-get-openapi.md
- name: Content API for Shopping - Get Product Status
  x-api-slug: merchantidproductstatuses-get
  description: Lists the statuses of the products in your Merchant Center account.
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidproductstatuses-get-openapi.md
- name: Content API for Shopping - Get Product Status
  x-api-slug: merchantidproductstatusesproductid-get
  description: Gets the status of a product from your Merchant Center account. This
    method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidproductstatusesproductid-get-openapi.md
- name: Content API for Shopping - Account Status Batch
  x-api-slug: accountstatusesbatch-post
  description: Retrieves account batch status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/accountstatusesbatch-post-openapi.md
- name: Content API for Shopping - Data Feed Status
  x-api-slug: datafeedstatusesbatch-post
  description: Retrieves data feed batch status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/datafeedstatusesbatch-post-openapi.md
- name: Content API for Shopping - Get Account Status
  x-api-slug: merchantidaccountstatuses-get
  description: Lists the statuses of the sub-accounts in your Merchant Center account.
    This method can only be called for multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidaccountstatuses-get-openapi.md
- name: Content API for Shopping - Get Account Status
  x-api-slug: merchantidaccountstatusesaccountid-get
  description: 'Retrieves the status of a Merchant Center account. This method can
    only be called for accounts to which the managing account has access: either the
    managing account itself or sub-accounts if the managing account is a multi-client
    account.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidaccountstatusesaccountid-get-openapi.md
- name: Content API for Shopping - Get Data Feed Status
  x-api-slug: merchantiddatafeedstatuses-get
  description: Lists the statuses of the datafeeds in your Merchant Center account.
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatuses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatuses-get-openapi.md
- name: Content API for Shopping - Get Data Feed Status
  x-api-slug: merchantiddatafeedstatusesdatafeedid-get
  description: Retrieves the status of a datafeed from your Merchant Center account.
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatusesdatafeedid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantiddatafeedstatusesdatafeedid-get-openapi.md
- name: Content API for Shopping - Get Product Status
  x-api-slug: merchantidproductstatuses-get
  description: Lists the statuses of the products in your Merchant Center account.
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidproductstatuses-get-openapi.md
- name: Content API for Shopping - Get Product Status
  x-api-slug: merchantidproductstatusesproductid-get
  description: Gets the status of a product from your Merchant Center account. This
    method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/google-content-api-for-shopping/merchantidproductstatusesproductid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.container.engine.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.content.api.for.shopping.stack.network
- type: x-best-practices
  url: https://developers.google.com/shopping-content/v2/best-practices
- type: x-code
  url: https://developers.google.com/shopping-content/v2/libraries
- type: x-testing
  url: https://developers.google.com/shopping-content/v2/how-tos/testing
- type: x-website
  url: https://developers.google.com/shopping-content/v2/quickstart
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---