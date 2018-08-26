{
  "info": {
    "name": "Vinli Get an Odometer Trigger",
    "_postman_id": "4809af9b-c626-4f5a-828b-719156a9233e",
    "description": "Get an odometer trigger.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Odometer",
      "item": [
        {
          "id": "0983474c-8395-4b97-abac-3bc709976b9a",
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
              "id": "44c51f9c-4963-4995-9cef-640b072b5fe9"
            }
          ]
        }
      ]
    }
  ]
}