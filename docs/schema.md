## users
column name     | data type | details
----------------|-----------|-----------------------
id              | integer   | not null, primary key
email           | string    | not null, unique
first_name      | string    | not null
last_name       | string    | not null
password_digest | string    | not null
session_token   | string    | not null, unique
skill_type      | string    | not null
gender          | string    | not null
city            | string    | not null

## user_views
column name     | data type | details
----------------|-----------|-----------------------
id              | integer   | not null, primary key
viewed_user_id  | string    | not null

<!-- how will picture storing work? -->
<!-- ## picture_posts
column name     | data type | details
----------------|-----------|-----------------------
id              | integer   | not null, primary key
user_id         | integer   | not null
caption         | string    |  -->

<!-- ## picture_likes
column name     | data type | details
----------------|-----------|-----------------------
id              | integer   | not null, primary key
liker_id        | integer   | not null
picture_id      | integer   | not null, (unique in context of liker_id)  -->
