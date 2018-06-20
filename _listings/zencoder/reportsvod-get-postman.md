{
  "info": {
    "name": "Zencoder API Get Usage for VOD",
    "_postman_id": "647fbd31-a4b2-442c-85e3-d22405f887bd",
    "description": "Get Usage for VOD",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "41052f51-2c61-4b40-9edd-d3fd5975d16f",
          "name": "getAccount",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Account Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ed547f5-3a11-4ce7-bb97-19fba01c43a6"
            }
          ]
        },
        {
          "id": "de812d18-4fff-4ec1-a6e1-ce602dee5482",
          "name": "postAccount",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account?email=%7B%7D&password=%7B%7D&password_confirmation=%7B%7D&terms_of_service=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a37059a-2499-4b41-b3d8-f9bf4f65f621"
            }
          ]
        },
        {
          "id": "9aceea9b-4ca3-441a-9b18-b269ebacbacc",
          "name": "putAccountIntegration",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account/integration?api_key=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Integration Mode"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb33b4a0-248f-46cb-b96e-8180a393b772"
            }
          ]
        },
        {
          "id": "6cadeef2-f793-4cc5-be75-3ec8a23cd743",
          "name": "putAccountLive",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account/live",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Integration Mode - Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "522886af-d746-4a78-a463-fe7faee68adb"
            }
          ]
        }
      ]
    },
    {
      "name": "Inputs",
      "item": [
        {
          "id": "0fc59d4f-17db-4d37-be8b-5dcd31d2f10c",
          "name": "getInupdatesInupdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "inputs/:input_id"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "input_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Input Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ac7930e-30f8-4ee0-b28f-16f75b1e4ecf"
            }
          ]
        },
        {
          "id": "7ce9c905-b8d8-4f2f-b293-46bd2668e67f",
          "name": "getInupdatesInupdateProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "inputs/:input_id/progress"
              ],
              "variable": [
                {
                  "id": "input_id",
                  "value": "input_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The return will contain one or more of the following keys: state, current_event, current_event_progress and progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f2b6636-b286-4ed4-b81f-8c346523f788"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "b0cb0a0e-e21b-414c-b21e-03d8b93634e0",
          "name": "getJobs",
          "request": {
            "url": "http://app.zencoder.com/api/v2/jobs?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of jobs can be obtained by sending an HTTP GET request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8a94374-359a-428d-9adc-6ac2d2a779b6"
            }
          ]
        },
        {
          "id": "50e77b9a-5359-4f7b-9ecd-48c595d125ff",
          "name": "postJobs",
          "request": {
            "url": "http://app.zencoder.com/api/v2/jobs?api_key=%7B%7D&Encoding Settings=%7B%7D&input=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Encoding jobs are created by sending an HTTP POST request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66f5d00d-635c-4bba-98aa-ee01b5bbcc83"
            }
          ]
        },
        {
          "id": "2cb7dc83-af45-4333-9921-bb3347a3f82b",
          "name": "getJobsJob",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Get Job Details",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "job_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Job Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5081467-a797-4d8e-b2fc-a4bab343bdcd"
            }
          ]
        },
        {
          "id": "d17e1e78-8c06-444a-b5b3-728570a2eaba",
          "name": "putJobsJobCancel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/cancel"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "If you wish to cancel a job that has not yet finished processing you may send a request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad9d6091-d49a-408a-8ae2-89699a031f4a"
            }
          ]
        },
        {
          "id": "f0da38c1-4a3f-4fc7-be34-029f3a5aabbb",
          "name": "putJobsJobFinish",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/finish"
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "job_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Finishes the input on a Live streaming job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c425c99-4560-43dc-82eb-a6f7ac970017"
            }
          ]
        },
        {
          "id": "951a6612-0311-43c3-a38b-d9c62f82a86a",
          "name": "getJobsJobProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/progress"
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "job_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The return will contain one or more of the following keys: state, input, outputs, and progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86ba8ef3-d774-4186-b930-d738c73bc4b7"
            }
          ]
        },
        {
          "id": "736a555e-7167-4e6b-9c1e-5b7f4c9a8978",
          "name": "putJobsJobResubmit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/resubmit"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "If a job has failed processing you may request that it be attempted again."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "388bad74-6475-4bf0-9a5d-b2e1863b5d96"
            }
          ]
        }
      ]
    },
    {
      "name": "Outputs",
      "item": [
        {
          "id": "5a836b6c-2d4e-4f80-b175-91d441c1f725",
          "name": "getOutupdatesOutupdateProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "outputs/:output_id/progress"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "output_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The return will contain one or more of the following keys: state, current_event, current_event_progress and progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68457938-583d-454f-b8c7-186c79458a0e"
            }
          ]
        }
      ]
    },
    {
      "name": "Reports",
      "item": [
        {
          "id": "9ba0dd97-77d5-42a0-b9de-235349dec799",
          "name": "getReportsAll",
          "request": {
            "url": "http://app.zencoder.com/api/v2/reports/all?api_key=%7B%7D&from=%7B%7D&grouping=%7B%7D&to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Usage for VOD & Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b91aeb0-fd94-4363-8271-78a2c79327ed"
            }
          ]
        },
        {
          "id": "d51624f3-f058-47de-890a-9be5deac5949",
          "name": "getReportsLive",
          "request": {
            "url": "http://app.zencoder.com/api/v2/reports/live?api_key=%7B%7D&from=%7B%7D&grouping=%7B%7D&to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Usage for Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3c68bda-d109-418e-a7b7-10685a4fc1bb"
            }
          ]
        },
        {
          "id": "ce89acce-558f-4a3a-8c4a-84239f8306dd",
          "name": "getReportsMinutes",
          "request": {
            "url": "http://app.zencoder.com/api/v2/reports/minutes?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Minutes Used"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4366430b-7e44-4026-b017-2c2e51b87c0b"
            }
          ]
        },
        {
          "id": "5698b491-c821-4312-bf94-76a2d8f4eef7",
          "name": "getReportsVod",
          "request": {
            "url": "http://app.zencoder.com/api/v2/reports/vod?api_key=%7B%7D&from=%7B%7D&grouping=%7B%7D&to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Usage for VOD"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27308be4-81cc-4824-bcb9-ec803ad72877"
            }
          ]
        }
      ]
    }
  ]
}