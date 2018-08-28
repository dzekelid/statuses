{
  "info": {
    "name": "World of Warcraft Get Realm Status",
    "_postman_id": "36f3484b-e454-481f-8aa6-bf3b921711c3",
    "description": "Retrieves realms status information. This information is limited to whether or not the realm is up, the type and state of the realm and the current population.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Character",
      "item": [
        {
          "id": "4d5acca6-b8ef-4274-9fa2-017f72c6f1d9",
          "name": "getCharacterRealmCharactername",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "character/:realm/:characterName"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "characterName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "realm",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single character at a time through an HTTP GET request to a URL describing the character profile resource. By default, a basic dataset will be returned and with each request and zero or more additional fields can be retrieved. The core dataset returned includes the character's realm, name, level, last modified timestamp, thumbnail, race id, achievement points value, gender id and class id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2aa69a39-0ea4-44a0-a75e-14c4f631b6c6"
            }
          ]
        }
      ]
    },
    {
      "name": "Guild",
      "item": [
        {
          "id": "9e6626db-e47d-444e-9c4b-36ba389d23b0",
          "name": "getGuildRealmGuildname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "guild/:realm/:guildName"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "guildName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "realm",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single guild at a time through an HTTP GET request to a url describing the guild profile resource. By default, a basic dataset will be returned and with each request and zero or more additional fields can be retrieved. The core dataset returned includes the guild's name, level, faction and achievement points."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbd3d241-4b62-4897-a4b2-4622ddfcdc1f"
            }
          ]
        }
      ]
    },
    {
      "name": "Realm",
      "item": [
        {
          "id": "d314d508-3e06-4b99-a109-87762ab3dbd1",
          "name": "getRealmStatus",
          "request": {
            "url": "http://us.battle.net/api/wow/realm/status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves realms status information. This information is limited to whether or not the realm is up, the type and state of the realm and the current population."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1bdd2d8-4726-46c1-9596-9d6f80d550ed"
            }
          ]
        }
      ]
    }
  ]
}