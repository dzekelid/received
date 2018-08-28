swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{username}/received_events:
    get:
      summary: Get Users Username Received Events
      description: These are events that you'll only see public events.
      operationId: these-are-events-that-youll-only-see-public-events
      x-api-path-slug: usersusernamereceived-events-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Received
      - Events
  /users/{username}/received_events/public:
    get:
      summary: Get Users Username Received Events Public
      description: List public events that a user has received
      operationId: list-public-events-that-a-user-has-received
      x-api-path-slug: usersusernamereceived-eventspublic-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Received
      - Events
      - Public