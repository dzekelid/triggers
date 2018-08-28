{
  "info": {
    "name": "Vinli Delete an Odometer Trigger",
    "_postman_id": "70c958f6-5468-46f2-ab32-f404de3c47df",
    "description": "Delete an odometer trigger.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Odometer",
      "item": [
        {
          "id": "42f7ae7e-b1f3-4535-a8b7-1b3c4f0b9e23",
          "name": "OdometerTriggersCe8f9a53906a4d39B06aD466d29a13f1Get",
          "request": {
            "url": "http://events.vin.li/api/v1/odometer_triggers/ce8f9a53-906a-4d39-b06a-d466d29a13f1",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get an odometer trigger."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "929eb044-a1b9-4ca4-9e3b-bf7fb7c0845d"
            }
          ]
        },
        {
          "id": "cf30f4be-88d1-4e44-97ed-a463804f1bcd",
          "name": "OdometerTriggersCe8f9a53906a4d39B06aD466d29a13f1Delete",
          "request": {
            "url": "http://events.vin.li/api/v1/odometer_triggers/ce8f9a53-906a-4d39-b06a-d466d29a13f1",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete an odometer trigger."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d2af55c-8d7f-4df8-9af4-79ea547e6fca"
            }
          ]
        }
      ]
    }
  ]
}