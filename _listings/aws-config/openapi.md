swagger: "2.0"
x-collection-name: AWS Config
x-complete: 1
info:
  title: AWS Config API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeConfigRuleEvaluationStatus:
    get:
      summary: Describe Config Rule Evaluation Status
      description: Returns status information for each of your AWS managed Config
        rules.
      operationId: describeConfigRuleEvaluationStatus
      x-api-path-slug: actiondescribeconfigruleevaluationstatus-get
      parameters:
      - in: query
        name: ConfigRuleNames
        description: The name of the AWS managed Config rules for which you want status
          information
        type: string
      - in: query
        name: Limit
        description: The number of rule evaluation results that you want returned
        type: string
      - in: query
        name: NextToken
        description: The NextToken string returned on a previous page that you use
          to get the next page of results in a paginated response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Evaluations
  /?Action=DescribeConfigurationRecorderStatus:
    get:
      summary: Describe Configuration Recorder Status
      description: Returns the current status of the specified configuration recorder.
      operationId: describeConfigurationRecorderStatus
      x-api-path-slug: actiondescribeconfigurationrecorderstatus-get
      parameters:
      - in: query
        name: ConfigurationRecorderNames
        description: The name(s) of the configuration recorder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Rules
  /?Action=DescribeDeliveryChannelStatus:
    get:
      summary: Describe Delivery Channel Status
      description: Returns the current status of the specified delivery channel.
      operationId: describeDeliveryChannelStatus
      x-api-path-slug: actiondescribedeliverychannelstatus-get
      parameters:
      - in: query
        name: DeliveryChannelNames
        description: A list of delivery channel names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Channels