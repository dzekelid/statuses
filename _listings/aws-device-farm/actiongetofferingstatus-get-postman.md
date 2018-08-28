{
  "info": {
    "name": "AWS Device Farm API Get Offering Status",
    "_postman_id": "be9a5e84-9fd8-4ac9-90d3-2a73f0d17415",
    "description": "Gets the current status and future status of all offerings purchased by an AWS account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "38488857-b947-4599-97b5-5dedb5c2ed6c",
          "name": "createDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=CreateDevicePool?description=description&name=name&projectArn=projectArn&rules=rules",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b75df35-cc51-4a63-bac5-fa80458ba5ea"
            }
          ]
        },
        {
          "id": "d59dff9b-8901-46ae-a2ad-f996131c40d9",
          "name": "deleteDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a device pool given the pool ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2b1e616-6c8c-4adc-b593-2eaf2bccb0df"
            }
          ]
        },
        {
          "id": "c884b1c6-b9a0-4981-8ce4-43e7c0e3df50",
          "name": "getDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b77992d-516c-478f-825b-a58bf1f65340"
            }
          ]
        },
        {
          "id": "d100dbbf-465c-4e42-b9b3-a38d606141dd",
          "name": "getDevicePoolCompatibility",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePoolCompatibility?appArn=appArn&devicePoolArn=devicePoolArn&testType=testType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about compatibility with a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1128595-d6c1-43f2-83bd-397152b009ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Project",
      "item": [
        {
          "id": "2dd5d5cc-3d50-469b-bb7e-d6c108e7d86b",
          "name": "createProject",
          "request": {
            "url": "http://example.com/api/?Action=CreateProject?name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ed000be-79b7-45df-8898-6f9a7ff31cc0"
            }
          ]
        }
      ]
    },
    {
      "name": "Remote Access Sessions",
      "item": [
        {
          "id": "ea535dc0-f5d4-47d3-b83f-7ddbe5455565",
          "name": "createRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=CreateRemoteAccessSession?configuration=configuration&deviceArn=deviceArn&name=name&projectArn=projectArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specifies and starts a remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e97a87d1-59d2-407f-a3d1-4acd826b224f"
            }
          ]
        },
        {
          "id": "c2c5174b-d35c-4c92-b41b-af68ffcccfc9",
          "name": "deleteRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a completed remote access session and its results."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf568bc7-c3af-44f6-916c-a40718bb8bca"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "508a0442-275e-4791-898f-e3dbff4f1a65",
          "name": "createUpload",
          "request": {
            "url": "http://example.com/api/?Action=CreateUpload?contentType=contentType&name=name&projectArn=projectArn&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads an app or test scripts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1a2daa2-ce4d-47b1-a356-e1f8ba7665a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "32e421f0-1360-4054-b631-f7fd1865dac3",
          "name": "deleteProject",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Device Farm project, given the project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "280dc8ab-0839-4c3b-a978-157c57b32b58"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "d1007a48-5304-4d95-a3dc-9b5ba6a4a0a3",
          "name": "deleteRun",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the run, given the run ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3d5d591-3a32-4901-af1c-e2dd8711a613"
            }
          ]
        }
      ]
    },
    {
      "name": "Uploads",
      "item": [
        {
          "id": "7a20188f-edb5-41d7-aa96-94773c7c6f70",
          "name": "deleteUpload",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an upload given the upload ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cdd553ee-4855-4eec-ba6e-5870abee7520"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Settings",
      "item": [
        {
          "id": "c89c9228-27c8-4328-98f7-8e86063c18e0",
          "name": "getAccountSettings",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountSettings?accountSettings=accountSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of unmetered iOS and/or unmetered Android devices that have been purchased by the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0de0691-ac92-4b5d-9af7-3dca740184d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "f3a27223-5880-48b9-9053-4f2b56c54ad1",
          "name": "getDevice",
          "request": {
            "url": "http://example.com/api/?Action=GetDevice?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a unique device type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82b61f2b-b026-46d4-9359-2b69a01839eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "719727b0-71f1-490c-9db4-6a8a502aab5b",
          "name": "getJob",
          "request": {
            "url": "http://example.com/api/?Action=GetJob?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7334f2c-3d29-4d60-bb25-a0e4e6fcec17"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Status",
      "item": [
        {
          "id": "b862915c-1ca6-4b76-b0b6-41bed95da243",
          "name": "getOfferingStatus",
          "request": {
            "url": "http://example.com/api/?Action=GetOfferingStatus?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the current status and future status of all offerings purchased by an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba2091fa-f9ff-486c-ba32-74fc5c20d3be"
            }
          ]
        }
      ]
    }
  ]
}