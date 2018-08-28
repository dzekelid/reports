{
  "info": {
    "name": "Zencoder API Get Usage for VOD & Live",
    "_postman_id": "e0e29b85-c02a-4f46-9076-ce78be6c54ef",
    "description": "Get Usage for VOD & Live",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "4b218747-7a3a-4b7d-b795-a5aeb3b32d88",
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
              "id": "e99afb3e-f762-4cd5-96e6-7ce30ec0ab3a"
            }
          ]
        },
        {
          "id": "90f52f0f-464f-49e5-ad09-f308f71541a3",
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
              "id": "a6ae5f2f-cb2d-45f2-b28b-09fde4b83206"
            }
          ]
        },
        {
          "id": "1983a10a-1f8e-4009-9f68-846d1a3ccf34",
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
              "id": "4900a3a6-5521-46fd-8ce2-8b62180b5657"
            }
          ]
        },
        {
          "id": "ea0606f4-1a12-4577-a2e3-3521381cdd95",
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
              "id": "c25d6ac2-dd0d-433d-a2f0-ceb61b09e3af"
            }
          ]
        }
      ]
    },
    {
      "name": "Inputs",
      "item": [
        {
          "id": "cc5e23f0-32ab-43db-9f3a-2c3c941a38d7",
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
              "id": "2c22a25a-7d5c-4fbf-96f4-f1d836d3828d"
            }
          ]
        },
        {
          "id": "7a663e83-d498-4aec-bafb-998d0cd79aee",
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
              "id": "0edaeb53-79d9-48d1-a3d6-78ffb9f0b48a"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "0e5603ce-cf12-4d88-854a-73c7f8bf3bdd",
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
              "id": "3ac6c4b9-198b-4f71-9b16-a65f70f08d3e"
            }
          ]
        },
        {
          "id": "cda1a8c3-843b-4c62-82bb-689f33e15830",
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
              "id": "c6c883b8-89e0-4a95-831f-32b202b70911"
            }
          ]
        },
        {
          "id": "8939f1f1-d608-4e24-b067-3af7039968a8",
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
              "id": "cd6aa8dc-8a4f-41c6-b255-76fde08fbcfb"
            }
          ]
        },
        {
          "id": "f32d21dc-f750-47b6-8a62-0dbb9293c002",
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
              "id": "84473eef-73b1-40c0-84d8-d0d0062e6158"
            }
          ]
        },
        {
          "id": "5ef53f8c-dae5-4a31-8d83-2113a688d9aa",
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
              "id": "39b43bd2-bf98-4214-ac79-2f74d5b914a2"
            }
          ]
        },
        {
          "id": "0779f76b-15ba-45e5-8c9d-52ab37b53a09",
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
              "id": "dcd9e360-06af-4f6c-a2c2-187d073d1738"
            }
          ]
        },
        {
          "id": "1f03023b-2e5e-4c00-aeba-c425912570b8",
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
              "id": "1f7ba36a-d81d-4847-9f89-ee09d02b273d"
            }
          ]
        }
      ]
    },
    {
      "name": "Outputs",
      "item": [
        {
          "id": "c4cf8f4e-657e-40a8-888a-c64de5278dfb",
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
              "id": "87cba575-5498-449f-b0e1-8f5ed2c34d9c"
            }
          ]
        }
      ]
    },
    {
      "name": "Reports",
      "item": [
        {
          "id": "8a998235-397c-4da7-b530-9877fdded9bf",
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
              "id": "638d17b2-e52e-40b2-b3b3-62470c1aebee"
            }
          ]
        }
      ]
    }
  ]
}