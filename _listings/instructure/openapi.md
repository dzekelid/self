swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/quizzes/quiz_id/submissions/self/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsselffiles-post
      parameters:
      - in: query
        name: name
        description: The name of the quiz submission file
      - in: query
        name: on_duplicate
        description: How to handle duplicate names
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Self
      - Files
  /users/self/activity_stream:
    delete:
      summary: Hide all stream items
      description: Hide all stream items.
      operationId: hide-all-stream-items
      x-api-path-slug: usersselfactivity-stream-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
    get:
      summary: List the activity stream
      description: List the activity stream.
      operationId: list-the-activity-stream
      x-api-path-slug: usersselfactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
  /users/self/activity_stream/summary:
    get:
      summary: Activity stream summary
      description: Activity stream summary.
      operationId: activity-stream-summary
      x-api-path-slug: usersselfactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
      - Summary
  /users/self/activity_stream/{id}:
    delete:
      summary: Hide a stream item
      description: Hide a stream item.
      operationId: hide-a-stream-item
      x-api-path-slug: usersselfactivity-streamid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
      - Id
  /users/self/bookmarks:
    get:
      summary: List bookmarks
      description: List bookmarks.
      operationId: list-bookmarks
      x-api-path-slug: usersselfbookmarks-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
    post:
      summary: Create bookmark
      description: Create bookmark.
      operationId: create-bookmark
      x-api-path-slug: usersselfbookmarks-post
      parameters:
      - in: query
        name: data
        description: The data associated with the bookmark
      - in: query
        name: name
        description: The name of the bookmark
      - in: query
        name: position
        description: The position of the bookmark
      - in: query
        name: url
        description: The url of the bookmark
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
  /users/self/bookmarks/{id}:
    delete:
      summary: Delete bookmark
      description: Delete bookmark.
      operationId: delete-bookmark
      x-api-path-slug: usersselfbookmarksid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
    get:
      summary: Get bookmark
      description: Get bookmark.
      operationId: get-bookmark
      x-api-path-slug: usersselfbookmarksid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
    put:
      summary: Update bookmark
      description: Update bookmark.
      operationId: update-bookmark
      x-api-path-slug: usersselfbookmarksid-put
      parameters:
      - in: query
        name: data
        description: The data associated with the bookmark
      - in: query
        name: name
        description: The name of the bookmark
      - in: query
        name: position
        description: The position of the bookmark
      - in: query
        name: url
        description: The url of the bookmark
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
  /users/self/communication_channels/{communication_channel_id}/notification_preferences:
    put:
      summary: Update multiple preferences
      description: Update multiple preferences.
      operationId: update-multiple-preferences
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preferences-put
      parameters:
      - in: query
        name: notification_preferences[X][frequency]
        description: The desired frequency for &lt;X&gt; notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
  /users/self/communication_channels/{communication_channel_id}/notification_preferences/notification:
    put:
      summary: Update a preference
      description: Update a preference.
      operationId: update-a-preference
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put
      parameters:
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for this notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
      - Notification
  /users/self/communication_channels/{communication_channel_id}/notification_preference_categories/category:
    put:
      summary: Update preferences by category
      description: Update preferences by category.
      operationId: update-preferences-by-category
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preference-categoriescategory-put
      parameters:
      - in: query
        name: category
        description: The name of the category
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for each notification in the category
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preference
      - Categories
      - Category
  /users/self/communication_channels/{type}/address/notification_preferences:
    put:
      summary: Update multiple preferences
      description: Update multiple preferences.
      operationId: update-multiple-preferences
      x-api-path-slug: usersselfcommunication-channelstypeaddressnotification-preferences-put
      parameters:
      - in: query
        name: notification_preferences[X][frequency]
        description: The desired frequency for &lt;X&gt; notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
  /users/self/communication_channels/{type}/address/notification_preferences/{notification}:
    put:
      summary: Update a preference
      description: Update a preference.
      operationId: update-a-preference
      x-api-path-slug: usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put
      parameters:
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for this notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
      - Notification
  /users/self/course_nicknames:
    delete:
      summary: Clear course nicknames
      description: Clear course nicknames.
      operationId: clear-course-nicknames
      x-api-path-slug: usersselfcourse-nicknames-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
    get:
      summary: List course nicknames
      description: List course nicknames.
      operationId: list-course-nicknames
      x-api-path-slug: usersselfcourse-nicknames-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
  /users/self/course_nicknames/{course_id}:
    delete:
      summary: Remove course nickname
      description: Remove course nickname.
      operationId: remove-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
    get:
      summary: Get course nickname
      description: Get course nickname.
      operationId: get-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
    put:
      summary: Set course nickname
      description: Set course nickname.
      operationId: set-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-put
      parameters:
      - in: query
        name: nickname
        description: The nickname to set
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
  /users/self/favorites/courses:
    delete:
      summary: Reset course favorites
      description: Reset course favorites.
      operationId: reset-course-favorites
      x-api-path-slug: usersselffavoritescourses-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
    get:
      summary: List favorite courses
      description: List favorite courses.
      operationId: list-favorite-courses
      x-api-path-slug: usersselffavoritescourses-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
  /users/self/favorites/courses/{id}:
    delete:
      summary: Remove course from favorites
      description: Remove course from favorites.
      operationId: remove-course-from-favorites
      x-api-path-slug: usersselffavoritescoursesid-delete
      parameters:
      - in: query
        name: id
        description: the ID or SIS ID of the course to remove
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
      - Id
    post:
      summary: Add course to favorites
      description: Add course to favorites.
      operationId: add-course-to-favorites
      x-api-path-slug: usersselffavoritescoursesid-post
      parameters:
      - in: query
        name: id
        description: The ID or SIS ID of the course to add
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
      - Id
  /users/self/favorites/groups:
    delete:
      summary: Reset group favorites
      description: Reset group favorites.
      operationId: reset-group-favorites
      x-api-path-slug: usersselffavoritesgroups-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
    get:
      summary: List favorite groups
      description: List favorite groups.
      operationId: list-favorite-groups
      x-api-path-slug: usersselffavoritesgroups-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
  /users/self/favorites/groups/{id}:
    delete:
      summary: Remove group from favorites
      description: Remove group from favorites.
      operationId: remove-group-from-favorites
      x-api-path-slug: usersselffavoritesgroupsid-delete
      parameters:
      - in: query
        name: id
        description: the ID or SIS ID of the group to remove
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
      - Id
    post:
      summary: Add group to favorites
      description: Add group to favorites.
      operationId: add-group-to-favorites
      x-api-path-slug: usersselffavoritesgroupsid-post
      parameters:
      - in: query
        name: id
        description: The ID or SIS ID of the group to add
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
      - Id
  /users/self/groups:
    get:
      summary: List your groups
      description: List your groups.
      operationId: list-your-groups
      x-api-path-slug: usersselfgroups-get
      parameters:
      - in: query
        name: context_type
        description: Only include groups that are in this type of context
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Groups
  /users/self/todo:
    get:
      summary: List the TODO items
      description: List the todo items.
      operationId: list-the-todo-items
      x-api-path-slug: usersselftodo-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Todo
  /users/self/upcoming_events:
    get:
      summary: List upcoming assignments, calendar events
      description: List upcoming assignments, calendar events.
      operationId: list-upcoming-assignments-calendar-events
      x-api-path-slug: usersselfupcoming-events-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Upcoming
      - Events