{
  "info": {
    "name": "Reddit Add Subreddit Accept Moderator Invite",
    "_postman_id": "b60d977f-51a8-49db-a88f-02db5794b4bb",
    "description": "Accept an invite to moderate the specified subreddit.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Best",
      "item": [
        {
          "id": "4ad5f7cb-58bb-42fb-9193-976699450339",
          "name": "get&nbsp;Best",
          "request": {
            "url": "http://www.reddit.com/best.json?after=after&before=before&count=count&limit=limit&show=show&sr_detail=sr_detail",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint is a listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16f4143c-4eb4-43e8-9b95-5760a3764d53"
            }
          ]
        }
      ]
    },
    {
      "name": "Names",
      "item": [
        {
          "id": "638be10f-8604-4f52-8934-a8e74db8dd84",
          "name": "get&nbsp;ByNames",
          "request": {
            "url": "http://www.reddit.com/by_id/names?names=names",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a listing of links by fullname."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05e98b17-7b95-484f-b1fd-4d8f2b49f80b"
            }
          ]
        }
      ]
    },
    {
      "name": "Subreddit",
      "item": [
        {
          "id": "89000928-f1c6-454b-9e32-d1bb60dd4277",
          "name": "get&nbsp;RSubredditHot",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.reddit.com",
              "path": [
                ":/r/subreddit/hot.json"
              ],
              "query": [
                {
                  "key": "after",
                  "value": "after",
                  "disabled": false
                },
                {
                  "key": "before",
                  "value": "before",
                  "disabled": false
                },
                {
                  "key": "count",
                  "value": "count",
                  "disabled": false
                },
                {
                  "key": "g",
                  "value": "g",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "limit",
                  "disabled": false
                },
                {
                  "key": "show",
                  "value": "show",
                  "disabled": false
                },
                {
                  "key": "sr_detail",
                  "value": "sr_detail",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "/r/subreddit",
                  "value": "/r/subreddit",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint is a listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c30ca0ce-d103-42da-add4-15e231086f87"
            }
          ]
        },
        {
          "id": "d89964bf-33e2-49b3-9528-a86d8ede77e5",
          "name": "get&nbsp;RSubredditNew",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.reddit.com",
              "path": [
                ":/r/subreddit/new.json"
              ],
              "query": [
                {
                  "key": "after",
                  "value": "after",
                  "disabled": false
                },
                {
                  "key": "before",
                  "value": "before",
                  "disabled": false
                },
                {
                  "key": "count",
                  "value": "count",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "limit",
                  "disabled": false
                },
                {
                  "key": "show",
                  "value": "show",
                  "disabled": false
                },
                {
                  "key": "sr_detail",
                  "value": "sr_detail",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "/r/subreddit",
                  "value": "/r/subreddit",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint is a listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd7d8a1b-1241-4814-8609-9c3ee8581177"
            }
          ]
        },
        {
          "id": "8e19cd93-b4e6-4559-b78a-40c970df5247",
          "name": "get&nbsp;RSubredditRandom",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.reddit.com",
              "path": [
                ":/r/subreddit/random.json"
              ],
              "variable": [
                {
                  "id": "/r/subreddit",
                  "value": "/r/subreddit",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Serendipity button"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2160965b-69e0-42f0-acde-e7354c6e2005"
            }
          ]
        },
        {
          "id": "2ae0f870-0dd8-40ac-8eec-28fb18fb484b",
          "name": "get&nbsp;RSubredditRising",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.reddit.com",
              "path": [
                ":/r/subreddit/rising.json"
              ],
              "query": [
                {
                  "key": "after",
                  "value": "after",
                  "disabled": false
                },
                {
                  "key": "before",
                  "value": "before",
                  "disabled": false
                },
                {
                  "key": "count",
                  "value": "count",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "limit",
                  "disabled": false
                },
                {
                  "key": "show",
                  "value": "show",
                  "disabled": false
                },
                {
                  "key": "sr_detail",
                  "value": "sr_detail",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "/r/subreddit",
                  "value": "/r/subreddit",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint is a listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5517209b-0d1e-4669-9dca-c7abace45e53"
            }
          ]
        },
        {
          "id": "8a9a0da5-4f26-4903-a08d-52c1d1fad900",
          "name": "get&nbsp;RSubredditSort",
          "request": {
            "url": "http://www.reddit.com/{/r/subreddit}/sort?after=after&before=before&count=count&limit=limit&show=show&sr_detail=sr_detail&t=t",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint is a listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "999419e6-b0b8-413a-b62e-d014cd45d5ea"
            }
          ]
        }
      ]
    }
  ]
}