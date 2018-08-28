{
  "info": {
    "name": "AWS Data Pipeline API Set Status",
    "_postman_id": "f19c7f49-7920-42a3-91d9-c6d60521debb",
    "description": "Requests that the status of the specified physical or logical pipeline objects be updated in the specified pipeline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "b62aade0-1bde-47e9-985a-0ca5c5ca8a21",
          "name": "activatePipeline",
          "request": {
            "url": "http://example.com/api/?Action=ActivatePipeline?parameterValues=parameterValues&pipelineId=pipelineId&startTimestamp=startTimestamp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Validates the specified pipeline and starts processing pipeline tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21bc9933-b2af-4887-a457-c279c0a153cc"
            }
          ]
        },
        {
          "id": "6e7db7f5-70e5-43b2-8a6f-7412949540b5",
          "name": "createPipeline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePipeline?description=description&name=name&tags=tags&uniqueId=uniqueId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new, empty pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94caa795-7801-4351-a155-4b2b8f42abe6"
            }
          ]
        },
        {
          "id": "4ae0795b-c18c-43e7-86af-bea2080ef994",
          "name": "deactivatePipeline",
          "request": {
            "url": "http://example.com/api/?Action=DeactivatePipeline?cancelActive=cancelActive&pipelineId=pipelineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deactivates the specified running pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c7aaee3-ea26-4548-9666-9bb37d7a32f5"
            }
          ]
        },
        {
          "id": "43028a95-9935-4d72-9e80-9df59bcd83a8",
          "name": "deletePipeline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePipeline?pipelineId=pipelineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a pipeline, its pipeline definition, and its run history."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df02e2f9-f09e-4974-a89b-ed2a903899e3"
            }
          ]
        },
        {
          "id": "d0c65fcc-275a-4396-ae0e-feaf7974fa73",
          "name": "describePipelines",
          "request": {
            "url": "http://example.com/api/?Action=DescribePipelines?pipelineIds=pipelineIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves metadata about one or more pipelines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f53a528c-1084-4b0f-8558-9c53147ae377"
            }
          ]
        },
        {
          "id": "1d8871b4-6a7d-40fd-b640-fa8fcea56795",
          "name": "getPipelineDefinition",
          "request": {
            "url": "http://example.com/api/?Action=GetPipelineDefinition?pipelineId=pipelineId&version=version",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the definition of the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa2dd1db-3691-47fd-852d-3649826b2a59"
            }
          ]
        },
        {
          "id": "f8ac1196-8ba8-4118-9430-722e6a8f90a3",
          "name": "listPipelines",
          "request": {
            "url": "http://example.com/api/?Action=ListPipelines?marker=marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the pipeline identifiers for all active pipelines that you have permission to access."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a840390-7ae9-4ae1-84fc-f695d0b7fb66"
            }
          ]
        },
        {
          "id": "e7a5a855-9458-4e63-82e9-2dd51486929b",
          "name": "putPipelineDefinition",
          "request": {
            "url": "http://example.com/api/?Action=PutPipelineDefinition?parameterObjects=parameterObjects&parameterValues=parameterValues&pipelineId=pipelineId&pipelineObjects=pipelineObjects",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds tasks, schedules, and preconditions to the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "039c94a6-8b08-4f68-a2bd-4f4a5099eb5c"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "4d13c208-ae79-4a4a-9107-2e756beb4bd6",
          "name": "addTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?pipelineId=pipelineId&tags=tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or modifies tags for the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37ac6573-48b5-455a-8e1e-e8c2f106eb37"
            }
          ]
        },
        {
          "id": "2546418c-0ee6-4bd5-b1a8-b23779a6e273",
          "name": "removeTags",
          "request": {
            "url": "http://example.com/api/?Action=RemoveTags?pipelineId=pipelineId&tagKeys=tagKeys",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes existing tags from the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "427851ca-e694-4c84-ba0e-b8d1a66fe619"
            }
          ]
        }
      ]
    },
    {
      "name": "Objects",
      "item": [
        {
          "id": "23702643-24c7-4afa-ace2-d41f3cfd3952",
          "name": "describeObjects",
          "request": {
            "url": "http://example.com/api/?Action=DescribeObjects?evaluateExpressions=evaluateExpressions&marker=marker&objectIds=objectIds&pipelineId=pipelineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the object definitions for a set of objects associated with the pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7f89416-e963-4be7-900d-b8c8db4cafe3"
            }
          ]
        },
        {
          "id": "4904d98c-6d11-46e6-988a-19442fafad26",
          "name": "queryObjects",
          "request": {
            "url": "http://example.com/api/?Action=QueryObjects?limit=limit&marker=marker&pipelineId=pipelineId&query=query&sphere=sphere",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Queries the specified pipeline for the names of objects that match the specified set of conditions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0254cb3b-18a1-4f16-9d58-50e99a60cd20"
            }
          ]
        }
      ]
    },
    {
      "name": "Expressions",
      "item": [
        {
          "id": "05e30cbf-9746-4093-af42-bb842041b19a",
          "name": "evaluateExpression",
          "request": {
            "url": "http://example.com/api/?Action=EvaluateExpression?expression=expression&objectId=objectId&pipelineId=pipelineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Task runners call EvaluateExpression to evaluate a string in the context of the specified object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "190a4e2b-ee27-4eb6-937e-c2bc51dda286"
            }
          ]
        }
      ]
    },
    {
      "name": "Tasks",
      "item": [
        {
          "id": "0dc12489-5007-4e2e-827e-212bbe9e5c4e",
          "name": "pollForTask",
          "request": {
            "url": "http://example.com/api/?Action=PollForTask?hostname=hostname&instanceIdentity=instanceIdentity&workerGroup=workerGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Task runners call PollForTask to receive a task to perform from AWS Data Pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "511084d0-16e3-4407-aaa6-b95dfb3ae8f3"
            }
          ]
        },
        {
          "id": "1e7ca317-d29c-45cb-919a-b4e8e910bfe4",
          "name": "reportTaskProgress",
          "request": {
            "url": "http://example.com/api/?Action=ReportTaskProgress?fields=fields&taskId=taskId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Task runners call ReportTaskProgress when assigned a task to acknowledge that it has the task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31ceaf2d-18fa-4d79-b103-a4ebe2eb77e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Task Runner Hearbeat",
      "item": [
        {
          "id": "1b4d3f5e-1991-4470-b5b9-a94009f4544c",
          "name": "reportTaskRunnerHeartbeat",
          "request": {
            "url": "http://example.com/api/?Action=ReportTaskRunnerHeartbeat?hostname=hostname&taskrunnerId=taskrunnerId&workerGroup=workerGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Task runners call ReportTaskRunnerHeartbeat every 15 minutes to indicate that they are operational."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65e96ff0-6372-4e72-b7c8-866cc0235865"
            }
          ]
        }
      ]
    },
    {
      "name": "Status",
      "item": [
        {
          "id": "e0917ad9-9f18-411d-bf88-5d91de0a575f",
          "name": "setStatus",
          "request": {
            "url": "http://example.com/api/?Action=SetStatus?objectIds=objectIds&pipelineId=pipelineId&status=status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests that the status of the specified physical or logical pipeline objects be updated in the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34713a90-97c2-4532-87b3-6989ae31a582"
            }
          ]
        }
      ]
    }
  ]
}