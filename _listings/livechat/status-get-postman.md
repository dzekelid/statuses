{
  "info": {
    "name": "LiveChat Get status",
    "_postman_id": "4bb0a761-413d-49c0-aa97-47ce966eb7af",
    "description": "Returns the current LiveChat status. Available return values: online, offline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhook",
      "item": [
        {
          "id": "8f0c6216-b035-4a3f-8eb7-bf616f59f002",
          "name": "Webhooks12345Delete",
          "request": {
            "url": "http://api.livechatinc.com/webhooks/12345",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a webhook with the given ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fad45aff-dcf9-4631-b076-806ea9250bd7"
            }
          ]
        }
      ]
    },
    {
      "name": "Chat",
      "item": [
        {
          "id": "734c6b2e-df4e-4acd-acd5-9a0d533402d4",
          "name": "ReportsChatsRatingsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/ratings?date_from=%7B%7D&date_to=%7B%7D&group=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows how many chats have been rated and how they have been rated during a specified period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15df2793-3afb-4285-9d13-7ad2337e6eb1"
            }
          ]
        },
        {
          "id": "3931cd38-5adf-4646-93a3-68f077a9e0c5",
          "name": "ReportsChatsEngagementGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/engagement?agent=%7B%7D&date_from=%7B%7D&date_to=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This report shows you where you get your chats from. They can come from i.e. automatic invitations, manual invitations or the visitors can start the chats by themselves."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e82e9e65-0a40-434d-84c6-e60666536ff7"
            }
          ]
        },
        {
          "id": "1c4de194-43c3-4c1a-af91-f6892bf7c05a",
          "name": "ReportsChatsRatingsRankingGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/ratings/ranking",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows the ratio of good to bad ratings for each operator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41d5327c-b41a-4a03-a01a-7ee88acf8d2a"
            }
          ]
        },
        {
          "id": "9a32c802-d19c-47c7-8d41-d26f9b7b777f",
          "name": "ChatsABC123TagsPut",
          "request": {
            "url": "http://api.livechatinc.com/chats/ABC123/tags",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "tag[0]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "tag[1]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "This method updates the tags assigned to a chat."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f0cef15-da7f-44ba-a51f-5711b41edf0b"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "592b3c51-8060-4a31-9805-15e58df8acaf",
          "name": "CannedResponsesABC123Get",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses/ABC123",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of all currently set canned responses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cb333db-f12a-42c9-b4c8-b931b91e4b27"
            }
          ]
        },
        {
          "id": "1e489e38-8ff2-45e4-860e-7ad2bfed04ed",
          "name": "GreetingsGet",
          "request": {
            "url": "http://api.livechatinc.com/greetings?groups=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of all greetings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee8437fb-0161-46d0-9708-6ae5015f8813"
            }
          ]
        },
        {
          "id": "46ebc167-a1df-47a5-a364-3aa59ad1c20f",
          "name": "TagsGet",
          "request": {
            "url": "http://api.livechatinc.com/tags?group=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns tags from all groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57627b2f-fee5-4ed4-9a89-84d89fa19eda"
            }
          ]
        },
        {
          "id": "26d66c77-ae77-4856-af22-3f3d3b659625",
          "name": "TicketsGet",
          "request": {
            "url": "http://api.livechatinc.com/tickets?date_from=%7B%7D&status=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all tickets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11c9c78f-f454-4468-a485-e42128e3f918"
            }
          ]
        },
        {
          "id": "c4845eec-6591-431c-a609-f855623122c4",
          "name": "CannedResponsesGet",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of all currently set canned responses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acab333b-d938-4e58-87cc-bdf181d848fa"
            }
          ]
        },
        {
          "id": "7fd80c1c-08a0-4a91-894f-a93666e89757",
          "name": "GroupsGet",
          "request": {
            "url": "http://api.livechatinc.com/groups",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all created groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2a1c520-dfa0-4f91-85b0-6d29886402a5"
            }
          ]
        },
        {
          "id": "738220ba-e72e-4313-b2fd-2cfcd635e36c",
          "name": "GoalsGet",
          "request": {
            "url": "http://api.livechatinc.com/goals",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all currently set goals. The active parameter indicates whether a goal is enabled or not."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c95e1e6-79da-465f-9167-60578ecb40fe"
            }
          ]
        },
        {
          "id": "4be8030a-3f97-4169-853e-b36c36aa95f6",
          "name": "ChatsGet",
          "request": {
            "url": "http://api.livechatinc.com/chats",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all ended chats."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4010f2a6-444c-4a43-b3ab-e4530fe2f3e0"
            }
          ]
        },
        {
          "id": "0776d42d-61f9-4384-9e20-9df23ef0a087",
          "name": "AgentsGet",
          "request": {
            "url": "http://api.livechatinc.com/agents",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all LiveChat agents list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ac96560-8947-43b7-a718-299649a16f1c"
            }
          ]
        },
        {
          "id": "71331558-f23c-4084-ad38-f036d7fe4356",
          "name": "VisitorsGet",
          "request": {
            "url": "http://api.livechatinc.com/visitors?group=%5B%7B%7D%5D&state=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the visitors on the pages with the tracking code installed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1eb93f95-880f-4844-8d79-fd2c53b9987f"
            }
          ]
        }
      ]
    },
    {
      "name": "Canned",
      "item": [
        {
          "id": "e059098a-3a4d-40d9-92dd-8678f89bd211",
          "name": "CannedResponsesABC123Put",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses/ABC123",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "tags[0]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Updates the specified canned response by setting the values of the parameters passed. Any parameters not provided will be left unchanged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1b515b6-824b-43ed-9d83-c4c98d06c129"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "0bef851b-cb85-401e-ac07-dfa5bab4e783",
          "name": "CannedResponsesABC123Delete",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses/ABC123",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Removes a canned response with the given CANNED_RESPONSE_ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "483bdaab-7fe1-4723-92c8-ac20fdc35fcf"
            }
          ]
        },
        {
          "id": "fee0ffd6-afc3-44f7-a821-34f4c079d1ef",
          "name": "GroupsABC123Delete2",
          "request": {
            "url": "http://api.livechatinc.com/groups/ABC123",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Removes a group with the given GROUP_ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5959f8a7-a7b5-4d42-8197-68be61f3979b"
            }
          ]
        },
        {
          "id": "d187058b-f7b9-4d23-94fa-40d3ed6aee46",
          "name": "AgentsJohnPublicComDelete",
          "request": {
            "url": "http://api.livechatinc.com/agents/john@public.com",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Removes an agent."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29e5cf00-fb70-4610-829e-93b0a4f8df04"
            }
          ]
        },
        {
          "id": "88618fb0-39de-4dba-920a-0740a2300404",
          "name": "GreetingsABC123Delete",
          "request": {
            "url": "http://api.livechatinc.com/greetings/ABC123",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Removes a greeting."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "887de821-ec91-4c92-93fc-113fb4da6791"
            }
          ]
        },
        {
          "id": "e364071b-d4fa-4264-8f01-352968865fe0",
          "name": "GoalsABC123Delete",
          "request": {
            "url": "http://api.livechatinc.com/goals/ABC123",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Removes a goal with the given GOAL_ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eea8b9f0-df51-42b6-a5e3-431cd083fbd2"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "30cb0c6e-b275-4c35-a319-0c01cfc8fed5",
          "name": "GroupsABC123Put",
          "request": {
            "url": "http://api.livechatinc.com/groups/ABC123",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "agents[0]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "agents[1]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Updates the specified group by setting the values of the parameters passed. Any parameters not provided will be left unchanged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51252c85-9d99-4db9-a0c7-6fdfef8e06f5"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "64ac7ce3-7d25-46e8-bd94-6257ea17ff5e",
          "name": "GreetingsPost",
          "request": {
            "url": "http://api.livechatinc.com/greetings",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[0][operator]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[0][type]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[0][value]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[1][operator]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[1][type]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[1][value]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Use this function to create a new greeting."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90b071f3-4692-48aa-b046-d164b84987ec"
            }
          ]
        },
        {
          "id": "d4b45720-2ecd-4398-9981-b3358ddd6808",
          "name": "WebhooksPost",
          "request": {
            "url": "http://api.livechatinc.com/webhooks",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "data_types",
                  "value": "[{}]",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "event_type",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Creates a new webhook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da957650-9574-4b27-bf36-66f2876c38f9"
            }
          ]
        },
        {
          "id": "d0b7014d-1f4e-4185-b4b7-b8cdd6a4bf68",
          "name": "CannedResponsesPost",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "tags[0]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "tags[1]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Creates a new canned response."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1862635-ea88-4dbc-a106-e9d9ca6edc71"
            }
          ]
        },
        {
          "id": "4ebf6f76-752c-4438-b276-4f594e6d752e",
          "name": "GroupsPost",
          "request": {
            "url": "http://api.livechatinc.com/groups",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "agents[0]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "agents[1]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Creates a new group in your license."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e7de7a5-a919-4f80-a15b-fe064fa688f8"
            }
          ]
        },
        {
          "id": "0f3495b9-c56f-4822-967d-be37251c07bd",
          "name": "GoalsPost",
          "request": {
            "url": "http://api.livechatinc.com/goals",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "match_type",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Creates a new goal."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "015f87c9-3fe5-446c-b34d-184301350c07"
            }
          ]
        },
        {
          "id": "af83cfce-5be3-4c39-a5ff-02dade89485a",
          "name": "AgentsPost",
          "request": {
            "url": "http://api.livechatinc.com/agents",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "login",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Creates a new agent in your license."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "450d7948-c4bc-43a3-96f9-45a1ccc12e6d"
            }
          ]
        }
      ]
    },
    {
      "name": "Display",
      "item": [
        {
          "id": "37cdc98d-bb86-4dbb-b8d3-96ce27df690e",
          "name": "WebhooksGet",
          "request": {
            "url": "http://api.livechatinc.com/webhooks",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of webhooks that have been created in a LiveChat account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aed5a603-9449-4d49-a66a-8b79d3bc8102"
            }
          ]
        }
      ]
    },
    {
      "name": "Greetings",
      "item": [
        {
          "id": "8fc5d38f-7ec3-4847-b73e-8ea7ab5cb2b8",
          "name": "ReportsChatsGreetingsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/greetings?date_from=%7B%7D&date_to=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the “greetings to chats to goals” conversion rates report.\n\ndisplayed is the number of displayed greetings. accepted tells you how many chats resulted from these greetings. goals tells you how many goals resulted from these greetings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a31809cd-daa0-4146-975d-79dc06ab0f03"
            }
          ]
        }
      ]
    },
    {
      "name": "Tag",
      "item": [
        {
          "id": "ec179183-03f9-464e-a438-647e5a758c76",
          "name": "TagsPost",
          "request": {
            "url": "http://api.livechatinc.com/tags",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "author",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "group",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "tag",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Adds a new tag. Note that only the owner and the admins are authorized to use this."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57143eb8-f0a3-4193-8066-501bf74301b8"
            }
          ]
        },
        {
          "id": "0450a88a-4a02-4921-b752-32e353e7daaf",
          "name": "TagsSupportDelete",
          "request": {
            "url": "http://api.livechatinc.com/tags/support",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "group",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Deletes a tag from the chosen group. The agents will no longer be able to tag chats and tickets using this tag.\n\nDeleting a tag will not remove it from the archived chats and tickets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b39bc02a-7692-4893-800a-38745b853a84"
            }
          ]
        }
      ]
    },
    {
      "name": "Single",
      "item": [
        {
          "id": "68e439ee-6f27-4e18-b3de-3831f368649b",
          "name": "AgentsJohnPublicComGet",
          "request": {
            "url": "http://api.livechatinc.com/agents/john@public.com",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns complete details of the agent for the given LOGIN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7074c647-f647-4895-8bff-62e1443786fb"
            }
          ]
        },
        {
          "id": "8cd624ca-85e1-4cb1-9849-df88e4ca0fbe",
          "name": "AgentsJohnPublicComPut",
          "request": {
            "url": "http://api.livechatinc.com/agents/john@public.com",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "job_title",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Returns complete details of the agent for the given LOGIN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5be2a120-a6b2-43f8-aaf2-3ee592c2e9e4"
            }
          ]
        },
        {
          "id": "88755a6a-7327-455e-8bca-c849094ce8a4",
          "name": "ChatsABC123Get",
          "request": {
            "url": "http://api.livechatinc.com/chats/ABC123",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single chat item for the given CHAT_ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1cd8ba2-febf-4f1f-8120-a25fca5fcb01"
            }
          ]
        },
        {
          "id": "6566aca8-d4af-4cf9-8cbe-7a9507cc366f",
          "name": "GreetingsABC123Get",
          "request": {
            "url": "http://api.livechatinc.com/greetings/ABC123",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the specified greeting."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7800d60-511f-4ad0-901b-f5b5160c6fca"
            }
          ]
        },
        {
          "id": "52d745ab-6648-49bb-9674-530b5a4407a6",
          "name": "GroupsByGroupIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.livechatinc.com",
              "path": [
                "groups/:group_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns group details for the given GROUP_ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30aba9b9-8915-4056-b795-f9b575c9a590"
            }
          ]
        },
        {
          "id": "14ca6b21-636d-4fe1-b934-cf6bda2cefe2",
          "name": "GoalsABC123Get",
          "request": {
            "url": "http://api.livechatinc.com/goals/ABC123",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the goal details for the given GOAL_ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f65ba35-f00f-446c-8c1d-3bd205e70ef0"
            }
          ]
        }
      ]
    },
    {
      "name": "Ticket",
      "item": [
        {
          "id": "839b6c85-9062-4f12-9a23-a287ba74a393",
          "name": "TicketsPost",
          "request": {
            "url": "http://api.livechatinc.com/tickets",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "message",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "requester[mail]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "requester[name]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "subject",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Creates a new ticket."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "295ab09c-d584-4c90-906b-8943de0cb6c2"
            }
          ]
        },
        {
          "id": "6ac1d51c-5f9b-4845-a0ba-805808f6bc3d",
          "name": "ReportsTicketsTicketSourcesGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/tickets/ticket_sources?date_from=%7B%7D&date_to=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows the distribution of the tickets between various channels."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7eccb032-f490-413d-8bc8-d2ab0034069e"
            }
          ]
        },
        {
          "id": "f971ba90-5878-4075-90af-a0250e304fd8",
          "name": "ReportsTicketsRatingsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/tickets/ratings?date_from=%7B%7D&date_to=%7B%7D&group=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows the tickets that were rated during the specified period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5be5cc1d-a94f-41b1-9880-e781cce9b728"
            }
          ]
        },
        {
          "id": "11642038-8754-4fb2-bb7f-fe38e220348a",
          "name": "Tickets5FUEDTagsPut",
          "request": {
            "url": "http://api.livechatinc.com/tickets/5FUED/tags",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "tag",
                  "value": "[{}]",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Updates tags associated with the ticket."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92d04011-efb9-43cf-addf-b416f97501b4"
            }
          ]
        },
        {
          "id": "906fcc3e-46f5-4360-ac92-5cabe177da1e",
          "name": "ReportsTicketsRatingsRankingGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/tickets/ratings/ranking",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows the ratio of good to bad ratings for each operator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c70e769c-dca3-4d46-8009-d3054b31181d"
            }
          ]
        }
      ]
    },
    {
      "name": "Solved",
      "item": [
        {
          "id": "a9927794-263a-4c44-8bdf-75bdc0a2255b",
          "name": "ReportsTicketsSolvedTicketsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/tickets/solved_tickets?date_from=%7B%7D&date_to=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows the number of the tickets solved during the specified period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a22b9c5d-d6e2-4fc5-9801-b42faa69fa1b"
            }
          ]
        }
      ]
    },
    {
      "name": "Chats",
      "item": [
        {
          "id": "9f8ffc2b-c84c-494c-8f78-4511ee0d5356",
          "name": "ReportsChatsFirstResponseTimeGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/first_response_time",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The average amount of time it takes the agents to respond to a new chat over a specified period of time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b78b5f6-22b2-4cb7-9fc1-5e8e2a39ca0b"
            }
          ]
        },
        {
          "id": "e80d7108-30d4-48d7-b3c8-5d0f66749061",
          "name": "ReportsChatsResponseTimeGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/response_time",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The average amount of time it takes the agents to respond to a new message in a chat during a specified period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b15a4597-93e7-41e8-941e-55d15e247f4c"
            }
          ]
        }
      ]
    },
    {
      "name": "Total",
      "item": [
        {
          "id": "57988bc3-48bb-412d-b800-1b6739ba47b0",
          "name": "ReportsChatsTotalChatsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/total_chats?agent=%7B%7D&date_from=%7B%7D&date_to=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows how many chats occurred during the specified period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18050004-0aa0-4157-8511-16e4d04ce5fd"
            }
          ]
        }
      ]
    },
    {
      "name": "Goal",
      "item": [
        {
          "id": "395ecc59-8c63-45ef-9325-948349c1c2c3",
          "name": "GoalsABC123Put",
          "request": {
            "url": "http://api.livechatinc.com/goals/ABC123",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Updates the specified goal by setting the values of the parameters passed. Any parameters not provided will be left unchanged.\n\nThe GOAL_ID is obtained from the goals list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35661fb3-76ed-4ba5-b9cf-ad6c1ea9ba0c"
            }
          ]
        }
      ]
    },
    {
      "name": "Availability",
      "item": [
        {
          "id": "e9764c9e-387c-45eb-81ee-442a42f7cf79",
          "name": "ReportsAvailabilityGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/availability",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows how long an agent (or a group or the whole account) was available for chatting during a specified period. When querying for one day, the results are shown in minutes per every hour, otherwise in hours for each day."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8030eb9-7aaa-447c-9c3b-2b52ff77322f"
            }
          ]
        }
      ]
    },
    {
      "name": "Tickets",
      "item": [
        {
          "id": "0a54332b-1e7b-466d-a0a0-b5762679d0a1",
          "name": "ReportsTicketsResolutionTimeGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/tickets/resolution_time?date_from=%7B%7D&date_to=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows the resolution time of the tickets that were solved during the specified period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08c25b16-7f7d-4821-b2a9-bb975d713839"
            }
          ]
        }
      ]
    },
    {
      "name": "Goals",
      "item": [
        {
          "id": "26dc0390-f7a1-4936-b4c0-bdd2255db6c8",
          "name": "ReportsChatsGoalsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/goals?date_from=%7B%7D&goal=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows the number of reached goals."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa2524dd-4df8-4fef-b9f4-8c2fe5c37a0b"
            }
          ]
        }
      ]
    },
    {
      "name": "Queued",
      "item": [
        {
          "id": "4ae3ce22-bc39-4f28-8292-62fd82a40e11",
          "name": "ReportsChatsQueuedVisitorsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/queued_visitors?date_from=%7B%7D&group=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows how many visitors waited in the queue and how many abandoned the queue or proceeded to chats"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fdca0d6-78f1-4b7f-8f52-c469737fea71"
            }
          ]
        }
      ]
    },
    {
      "name": "Queue",
      "item": [
        {
          "id": "afcbea01-531f-4039-a0e3-4e35b33b58d3",
          "name": "ReportsChatsQueuedVisitorsWaitingTimesGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/queued_visitors/waiting_times?date_from=%7B%7D&group=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows the Minimum, Average and Maximum waiting time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "850bf51c-5af1-4100-8130-bdf4703a717f"
            }
          ]
        }
      ]
    },
    {
      "name": "Chatting",
      "item": [
        {
          "id": "2ba3ae36-5360-42d3-8573-63555103d0ed",
          "name": "ReportsChatsChattingTimeGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/chatting_time",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows how much time an agent (or a group) spent on chatting during a specified period. When querying for one day, the results are shown in minutes per every hour, otherwise in hours for each day."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b293aec-7459-433c-8852-859c39428ab5"
            }
          ]
        }
      ]
    },
    {
      "name": "Mark",
      "item": [
        {
          "id": "828c6829-b201-490b-b8b6-