---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Post Users Self Update
  description: /users/{USER_ID}/unfriend
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/self/update:
    post:
      summary: Post Users Self Update
      description: /users/{USER_ID}/unfriend
      operationId: usersuser-idunfriend
      x-api-path-slug: usersselfupdate-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: photo
        description: Photo under 100KB in multipart MIME encoding with content type
          image/jpeg, image/gif, or image/png
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
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