swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
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