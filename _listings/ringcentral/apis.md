---
name: RingCentral
x-slug: ringcentral
description: 'RingCentral, Inc. (NYSE: RNG) is a global provider of cloud enterprise
  unified communications and collaboration solutions. More flexible and cost-effective
  than legacy on-premise systems, RingCentral empowers today&rsquo;s mobile and distributed
  workforces to be connected anywhere and on any device through voice, video, team
  messaging, collaboration, SMS, conferencing, online meetings, contact center, and
  fax. RingCentral provides an open platform that integrates with today&rsquo;s leading
  business apps while giving customers the flexibility to customize their own workflows.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
x-kinRank: "7"
x-alexaRank: "7180"
tags: Statuses
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/apis.md
specificationVersion: "0.14"
apis:
- name: RingCentral Connect Platform API Explorer - Get Service status
  x-api-slug: restapiv1-0status-get
  description: |-
    Returns current PAS service status.
    Usage Plan Group
    NoThrottling
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0status-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0status-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Status of RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
  description: "Returns the status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n503\nCMN-201\nService Temporary Unavailable"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Status of RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
  description: "Returns status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [RingOut] permission\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Status
  x-api-slug: restapiv1-0accountaccountidextensionextensionidpresence-get
  description: "Returns presence status of an extension or several extensions by their
    ID(s). Batch request is supported. The &#39;presenceStatus&#39; is returned as
    Offline (the parameters &#39;telephonyStatus&#39;, &#39;message&#39;, &#39;userStatus&#39;
    and &#39;dndStatus&#39; are not returned at all) for the following extension types:
    Department/Announcement Only/Take Messages Only (Voicemail)/Fax User/Paging Only
    Group/Shared Lines Group/IVR Menu/Application Extension/Park Location.If the user
    requests his/her own presence status, the response contains actual presence status
    even if the status publication is turned off. Batch request is supported. For
    batch requests the number of extensions in one request is limited to 30. If more
    extensions are included in the request, the error code 400 Bad Request is returned
    with the logical error code InvalidMultipartRequest and the corresponding message
    &#39;Extension Presence Info multipart request is limited to 30 extensions&#39;.\nApp
    Permission\nReadPresence\nUser Permission\nReadPresenceStatus\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadPresenceStatus] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidpresence-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update User Status
  x-api-slug: restapiv1-0accountaccountidextensionextensionidpresence-put
  description: "Updates user-defined extension presence status, status message and
    DnD status by extension ID. Supported for regular User extensions only. The extension
    types listed do not support presence status: Department, Announcement Only, Take
    Messages Only (Voicemail), Fax User, Paging Only Group, Shared Lines Group, IVR
    Menu, Application Extension.\nApp Permission\nEditPresence\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [allowSeeMyPresence] value is invalid\n\n\n403\nBIL-103\nFeature [DND] is not
    available for current account\n\n\n403\nCMN-408\nIn order to call this API endpoint,
    user needs to have [EditPresenceSettings] permission for requested resource.\n\n\n403\nPRS-105\nNot
    allowed update presence for extensions having Disabled state\n\n\n403\nPRS-106\nNot
    allowed update presence for extensions of Department type\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidpresence-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Service status
  x-api-slug: restapiv1-0status-get
  description: |-
    Returns current PAS service status.
    Usage Plan Group
    NoThrottling
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0status-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0status-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Status of RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
  description: "Returns the status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n503\nCMN-201\nService Temporary Unavailable"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Status of RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
  description: "Returns status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [RingOut] permission\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Status
  x-api-slug: restapiv1-0accountaccountidextensionextensionidpresence-get
  description: "Returns presence status of an extension or several extensions by their
    ID(s). Batch request is supported. The &#39;presenceStatus&#39; is returned as
    Offline (the parameters &#39;telephonyStatus&#39;, &#39;message&#39;, &#39;userStatus&#39;
    and &#39;dndStatus&#39; are not returned at all) for the following extension types:
    Department/Announcement Only/Take Messages Only (Voicemail)/Fax User/Paging Only
    Group/Shared Lines Group/IVR Menu/Application Extension/Park Location.If the user
    requests his/her own presence status, the response contains actual presence status
    even if the status publication is turned off. Batch request is supported. For
    batch requests the number of extensions in one request is limited to 30. If more
    extensions are included in the request, the error code 400 Bad Request is returned
    with the logical error code InvalidMultipartRequest and the corresponding message
    &#39;Extension Presence Info multipart request is limited to 30 extensions&#39;.\nApp
    Permission\nReadPresence\nUser Permission\nReadPresenceStatus\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadPresenceStatus] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidpresence-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update User Status
  x-api-slug: restapiv1-0accountaccountidextensionextensionidpresence-put
  description: "Updates user-defined extension presence status, status message and
    DnD status by extension ID. Supported for regular User extensions only. The extension
    types listed do not support presence status: Department, Announcement Only, Take
    Messages Only (Voicemail), Fax User, Paging Only Group, Shared Lines Group, IVR
    Menu, Application Extension.\nApp Permission\nEditPresence\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [allowSeeMyPresence] value is invalid\n\n\n403\nBIL-103\nFeature [DND] is not
    available for current account\n\n\n403\nCMN-408\nIn order to call this API endpoint,
    user needs to have [EditPresenceSettings] permission for requested resource.\n\n\n403\nPRS-105\nNot
    allowed update presence for extensions having Disabled state\n\n\n403\nPRS-106\nNot
    allowed update presence for extensions of Department type\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidpresence-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Update User Status
  x-api-slug: restapiv1-0accountaccountidextensionextensionidpresence-put
  description: "Updates user-defined extension presence status, status message and
    DnD status by extension ID. Supported for regular User extensions only. The extension
    types listed do not support presence status: Department, Announcement Only, Take
    Messages Only (Voicemail), Fax User, Paging Only Group, Shared Lines Group, IVR
    Menu, Application Extension.\nApp Permission\nEditPresence\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [allowSeeMyPresence] value is invalid\n\n\n403\nBIL-103\nFeature [DND] is not
    available for current account\n\n\n403\nCMN-408\nIn order to call this API endpoint,
    user needs to have [EditPresenceSettings] permission for requested resource.\n\n\n403\nPRS-105\nNot
    allowed update presence for extensions having Disabled state\n\n\n403\nPRS-106\nNot
    allowed update presence for extensions of Department type\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidpresence-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Update User Status
  x-api-slug: restapiv1-0accountaccountidextensionextensionidpresence-put
  description: "Updates user-defined extension presence status, status message and
    DnD status by extension ID. Supported for regular User extensions only. The extension
    types listed do not support presence status: Department, Announcement Only, Take
    Messages Only (Voicemail), Fax User, Paging Only Group, Shared Lines Group, IVR
    Menu, Application Extension.\nApp Permission\nEditPresence\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [allowSeeMyPresence] value is invalid\n\n\n403\nBIL-103\nFeature [DND] is not
    available for current account\n\n\n403\nCMN-408\nIn order to call this API endpoint,
    user needs to have [EditPresenceSettings] permission for requested resource.\n\n\n403\nPRS-105\nNot
    allowed update presence for extensions having Disabled state\n\n\n403\nPRS-106\nNot
    allowed update presence for extensions of Department type\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidpresence-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Status
  x-api-slug: restapiv1-0accountaccountidextensionextensionidpresence-get
  description: "Returns presence status of an extension or several extensions by their
    ID(s). Batch request is supported. The &#39;presenceStatus&#39; is returned as
    Offline (the parameters &#39;telephonyStatus&#39;, &#39;message&#39;, &#39;userStatus&#39;
    and &#39;dndStatus&#39; are not returned at all) for the following extension types:
    Department/Announcement Only/Take Messages Only (Voicemail)/Fax User/Paging Only
    Group/Shared Lines Group/IVR Menu/Application Extension/Park Location.If the user
    requests his/her own presence status, the response contains actual presence status
    even if the status publication is turned off. Batch request is supported. For
    batch requests the number of extensions in one request is limited to 30. If more
    extensions are included in the request, the error code 400 Bad Request is returned
    with the logical error code InvalidMultipartRequest and the corresponding message
    &#39;Extension Presence Info multipart request is limited to 30 extensions&#39;.\nApp
    Permission\nReadPresence\nUser Permission\nReadPresenceStatus\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadPresenceStatus] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidpresence-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Status
  x-api-slug: restapiv1-0accountaccountidextensionextensionidpresence-get
  description: "Returns presence status of an extension or several extensions by their
    ID(s). Batch request is supported. The &#39;presenceStatus&#39; is returned as
    Offline (the parameters &#39;telephonyStatus&#39;, &#39;message&#39;, &#39;userStatus&#39;
    and &#39;dndStatus&#39; are not returned at all) for the following extension types:
    Department/Announcement Only/Take Messages Only (Voicemail)/Fax User/Paging Only
    Group/Shared Lines Group/IVR Menu/Application Extension/Park Location.If the user
    requests his/her own presence status, the response contains actual presence status
    even if the status publication is turned off. Batch request is supported. For
    batch requests the number of extensions in one request is limited to 30. If more
    extensions are included in the request, the error code 400 Bad Request is returned
    with the logical error code InvalidMultipartRequest and the corresponding message
    &#39;Extension Presence Info multipart request is limited to 30 extensions&#39;.\nApp
    Permission\nReadPresence\nUser Permission\nReadPresenceStatus\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadPresenceStatus] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidpresence-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Status of RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
  description: "Returns status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [RingOut] permission\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Status of RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
  description: "Returns status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [RingOut] permission\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Status of RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
  description: "Returns the status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n503\nCMN-201\nService Temporary Unavailable"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Status of RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
  description: "Returns the status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n503\nCMN-201\nService Temporary Unavailable"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Service status
  x-api-slug: restapiv1-0status-get
  description: |-
    Returns current PAS service status.
    Usage Plan Group
    NoThrottling
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0status-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0status-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Service status
  x-api-slug: restapiv1-0status-get
  description: |-
    Returns current PAS service status.
    Usage Plan Group
    NoThrottling
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0status-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0status-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Service status
  x-api-slug: restapiv1-0status-get
  description: |-
    Returns current PAS service status.
    Usage Plan Group
    NoThrottling
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0status-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/ringcentral/restapiv1-0status-get-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/ringcentral-developers
- type: x-blog-rss
  url: https://medium.com/feed/ringcentral-developers
- type: x-github
  url: https://github.com/ringcentral
- type: x-openapi
  url: https://netstorage.ringcentral.com/dpw/api-explorer/swagger-ring_basic.yml?v=20180816
- type: x-website
  url: http://www.ringcentral.com
- type: x-api-gallery
  url: http://reverb.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ringcentral.stack.network
- type: x-code
  url: https://developer.ringcentral.com/library/sdks.html
- type: x-crunchbase
  url: https://crunchbase.com/organization/ringcentral
- type: x-developer
  url: https://developer.ringcentral.com/
- type: x-documentation
  url: https://developer.ringcentral.com/api-explorer/latest/index.html?_ga=2.259782990.551967760.1534465156-1236351744.1533920460
- type: x-support
  url: https://developer.ringcentral.com/support.html
- type: x-twitter
  url: https://twitter.com/RingCentral
- type: x-website
  url: https://developer.ringcentral.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---