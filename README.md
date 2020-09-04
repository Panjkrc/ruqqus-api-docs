# Ruqqus API DOCUMENTATION
## Get started using the API

I'm not goint to go into details abot how to create an app and get all the neccesarry keys, necause there already exists [a guide on that](https://ruqqus.com/help/oauth)

## List of all current endpoints, their corresponding parameters and the values they return:

### JSON API
<hr>

### `/api/v1/guild/<boardname>`
  Description: Get guild data  
  • method: `GET`  
  • requiers oauth: `TRUE`  
  • scope required: `READ`  
  • returns (JSON):  
  
  ```json
  {
    "banner_url": "https://i.ruqqus.com/board/ruqqusapi/banner-3.png",
    "color": "#2A96F3",
    "created_utc": 1598948139,
    "description": "A place to discuss Ruqqus API, ask questions and post \"500 (Internal server error)\" memes",
    "description_html": "<p>A place to discuss Ruqqus API, ask questions and post \"500 (Internal server error)\" memes</p>\n",
    "fullname": "t4_3my",
    "id": "3my",
    "is_banned": false,
    "is_private": false,
    "is_restricted": false,
    "mods_count": 5,
    "name": "RuqqusAPI",
    "over_18": false,
    "permalink": "/+RuqqusAPI",
    "profile_url": "https://i.ruqqus.com/board/ruqqusapi/profile-1.png",
    "subscriber_count": 22
}
  ```
  
### `/api/v1/user/<username>`
  Description: Get user data  
  • method: `GET`  
  • requiers oauth: `TRUE`  
  • scope required: `READ`  
  • returns (JSON):  
  
  ```json
  {
    "badges": [{
        "created_utc": 1567773596,
        "name": "Verified Email",
        "text": "Verified Email",
        "url": null
    }, {
        "created_utc": null,
        "name": "Alpha User",
        "text": "Joined Ruqqus during open alpha",
        "url": null
    }, {
        "created_utc": null,
        "name": "Code Contributor",
        "text": "Contributed to Ruqqus source code",
        "url": null
    }, {
        "created_utc": 1591719748,
        "name": "Sitebreaker",
        "text": "Inadvertantly broke Ruqqus",
        "url": null
    }],
    "banner_url": "https://i.ruqqus.com/users/captainmeta4/banner-2.png",
    "bio": "Ruqqus co-founder and lead backend dev\r\n\r\nhttps://github.com/captainmeta4",
    "bio_html": "<p>Ruqqus co-founder and lead backend dev</p>\n<p><a href=\"https://github.com/captainmeta4\" rel=\"nofollow noopener\" target=\"_blank\">https://github.com/captainmeta4</a></p>\n",
    "comment_count": 1933,
    "comment_rep": 8392,
    "created_utc": 1562447012,
    "id": "7",
    "is_banned": false,
    "permalink": "/@captainmeta4",
    "post_count": 348,
    "post_rep": 12857,
    "profile_url": "https://i.ruqqus.com/users/captainmeta4/profile-6.png",
    "title": {
        "color": "#5555dd",
        "id": 5,
        "kind": 3,
        "text": " the Codesmith"
    },
    "username": "captainmeta4"
}
  ```
  
### `/api/v1/post/<pid>`
  Description: Get post data   
  • method: `GET`  
  • requiers oauth: `TRUE`  
  • scope required: `READ`  
  • returns (JSON):  
  
  ```json
  {
    "author": "movie",
    "author_title": {
        "color": "#5555dd",
        "id": 21,
        "kind": 1,
        "text": " the Friendly"
    },
    "body": "Currently there is no official documentation for Ruqqus API but there is a help page on how to get started with it: https://ruqqus.com/help/oauth   \r\n\r\nYou can search through [Ruqqus's GitHub page](https://github.com/ruqqus/ruqqus) to find all of the routes.  \r\nMore specifically: https://github.com/ruqqus/ruqqus/tree/master/ruqqus/routes  \r\n\r\nWe are planing to make our own documentation that will include all of the routes/endpoints and their corresponding parameters that will serve until official one gets released",
    "body_html": "<p>Currently there is no official documentation for Ruqqus API but there is a help page on how to get started with it: <a href=\"https://ruqqus.com/help/oauth\">https://ruqqus.com/help/oauth</a></p>\n<p>You can search through <a href=\"https://github.com/ruqqus/ruqqus\" rel=\"nofollow noopener\" target=\"_blank\">Ruqqus's GitHub page</a> to find all of the routes.  \nMore specifically: <a href=\"https://github.com/ruqqus/ruqqus/tree/master/ruqqus/routes\" rel=\"nofollow noopener\" target=\"_blank\">https://github.com/ruqqus/ruqqus/tree/master/ruqqus/routes</a></p>\n<p>We are planing to make our own documentation that will include all of the routes/endpoints and their corresponding parameters that will serve until official one gets released</p>\n",
    "comment_count": 3,
    "created_utc": 1598950552,
    "domain": "text post",
    "downvotes": 0,
    "edited_utc": 1598950710,
    "embed_url": "",
    "fullname": "t2_2v0b",
    "guild_name": "RuqqusAPI",
    "id": "2v0b",
    "is_archived": false,
    "is_banned": false,
    "is_deleted": false,
    "is_nsfl": false,
    "is_nsfw": false,
    "original_guild_name": "RuqqusAPI",
    "permalink": "/post/2v0b/how-to-get-started-using-ruqqus",
    "score": 16,
    "thumb_url": null,
    "title": "How to get started using Ruqqus API",
    "upvotes": 14,
    "url": "",
    "voted": 0
}
  ```
  
### `/api/v1/comment/<cid>`
  Description: Get comment data
  • method: `GET`  
  • requiers oauth: `TRUE`  
  • scope required: `READ`  
  • returns (JSON):  
  
  ```json
  {
    "author": "kek",
    "body": "Good bot",
    "body_html": "<p>Good bot</p>\n",
    "created_utc": 1599077272,
    "downvotes": 0,
    "edited_utc": 0,
    "fullname": "t3_a3td",
    "guild_name": "RuqqusAPI",
    "id": "a3td",
    "is_archived": false,
    "is_banned": false,
    "is_deleted": false,
    "is_nsfl": false,
    "is_nsfw": false,
    "is_offensive": false,
    "level": 1,
    "parent": "t2_2wrn",
    "permalink": "/post/2wrn/this-is-a-test-post/a3td",
    "post": "2wrn",
    "score": 4,
    "title": {
        "color": "#5555dd",
        "id": 5,
        "kind": 3,
        "text": " the Codesmith"
    },
    "upvotes": 4
}  
  ```
  
<hr>

### BOARDS(guilds) API
<hr>

### `/api/board_available/<name>`
  Description: Check if guild name is available
  • method: `GET`  
  • requiers oauth: `FALSE`    
  • returns (JSON):  
  
  ```json
  {"available":false,"board":"RuqqusAPI"}
  ```
  
### `
