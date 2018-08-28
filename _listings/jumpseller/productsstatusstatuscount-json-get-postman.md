{
  "info": {
    "name": "Jumpseller Get Products Status Status Count",
    "_postman_id": "7a4e4b60-6849-45d9-be7c-0b0b737c52b8",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "dde13b87-916e-4dbc-935a-134de28044d9",
          "name": "getCountries.json",
          "request": {
            "url": "http://api.jumpseller.com/v1/countries.json?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all countries.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46b1a1b6-c26f-4e19-8377-6ab44d96437e"
            }
          ]
        },
        {
          "id": "fead352a-e5e1-4250-b47c-3ed6ccd2af44",
          "name": "getCountriesCountryCode.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "countries/:country_code.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "country_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a single country information.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "618fe675-ed7a-436d-bf68-dc0281dc97bc"
            }
          ]
        },
        {
          "id": "5c8ec2be-d427-4d31-a8e4-fdeaa8f65298",
          "name": "getCountriesCountryCodeRegions.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "countries/:country_code/regions.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "country_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all regions from a single country.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8eb2465-3752-4ba4-8ab2-e3b44261b7b7"
            }
          ]
        },
        {
          "id": "4145c823-fca0-42da-9f54-bf2098f2943d",
          "name": "getCountriesCountryCodeRegionsRegionCode.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "countries/:country_code/regions/:region_code.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "country_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "region_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a single region information object.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5d1e185-1e39-4ad6-8b79-f16651799756"
            }
          ]
        }
      ]
    },
    {
      "name": "Products",
      "item": [
        {
          "id": "709dd90d-9c7c-4f27-a963-a324df124f23",
          "name": "getProductsCategoryCategoryCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/category/:category_id/count.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "category_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Category Category Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e13b692e-ffcf-4d4b-b653-48fdc29ae131"
            }
          ]
        },
        {
          "id": "fcdf78c1-ad2f-4f07-bdfc-7f0608f2ba09",
          "name": "getProductsCount.json",
          "request": {
            "url": "http://api.jumpseller.com/v1/products/count.json?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6341d8ff-65e7-43b1-bccf-09e5de3ae7d9"
            }
          ]
        },
        {
          "id": "ff800623-f795-46ba-b729-c1a45bb81c02",
          "name": "getProductsStatusStatusCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/status/:status/count.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "status",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Status Status Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64fb37db-37c2-4f38-a126-c41944615e93"
            }
          ]
        }
      ]
    }
  ]
}