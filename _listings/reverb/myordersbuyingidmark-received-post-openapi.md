---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Post My Orders Buying Mark Received
  description: Marks an order as received by the buyer
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/feedback/received:
    get:
      summary: Get My Feedback Received
      description: List of received feedback
      operationId: getMyFeedbackReceived
      x-api-path-slug: myfeedbackreceived-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Feedback
      - Received
  /my/orders/buying/{id}/mark_received:
    post:
      summary: Post My Orders Buying Mark Received
      description: Marks an order as received by the buyer
      operationId: postMyOrdersBuyingMarkReceived
      x-api-path-slug: myordersbuyingidmark-received-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
      - Id
      - Mark
      - Received
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---