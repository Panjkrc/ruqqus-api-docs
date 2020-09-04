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
  
### `/api/v1/guild/<name>/listing`
  Description: Get guild listing    
  • method: `GET`  
  • requiers oauth: `TRUE`  
  • scope required: `READ`  
  • returns (JSON):  
  
  ```json
  {
    "data": [{
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
        "score": 14,
        "thumb_url": null,
        "title": "How to get started using Ruqqus API",
        "upvotes": 16,
        "url": "",
        "voted": 1
    }, {
        "author": "SuperLeaf1995",
        "author_title": {
            "color": "#aa8855",
            "id": 11,
            "kind": 1,
            "text": ", Guildsmith"
        },
        "body": "This is an unofficial API guide, written in good faith to help everyone in their journey to making bots and/or APIs.\r\n\r\nIncludes two sections: One for API developers and other for Bot developers.\r\n\r\nThis explains several important stuff of the Ruqqus API.\r\n\r\nI hope this PDF is useful for API/Bot devs ;).",
        "body_html": "<p>This is an unofficial API guide, written in good faith to help everyone in their journey to making bots and/or APIs.</p>\n<p>Includes two sections: One for API developers and other for Bot developers.</p>\n<p>This explains several important stuff of the Ruqqus API.</p>\n<p>I hope this PDF is useful for API/Bot devs ;).</p>\n",
        "comment_count": 0,
        "created_utc": 1599168920,
        "domain": "drive.google.com",
        "downvotes": 0,
        "edited_utc": 0,
        "embed_url": "",
        "fullname": "t2_2y1f",
        "guild_name": "RuqqusAPI",
        "id": "2y1f",
        "is_archived": false,
        "is_banned": false,
        "is_deleted": false,
        "is_nsfl": false,
        "is_nsfw": false,
        "original_guild_name": "RuqqusAPI",
        "permalink": "/post/2y1f/api-guide-for-bot-and-api",
        "score": 4,
        "thumb_url": null,
        "title": "API Guide for bot and API developers",
        "upvotes": 4,
        "url": "https://drive.google.com/file/d/1EGSuDSPShxEHEjGz1NJ1K7VcXqpanVQy/view?usp=sharing",
        "voted": 1
    }, {
        "author": "movie",
        "author_title": {
            "color": "#5555dd",
            "id": 21,
            "kind": 1,
            "text": " the Friendly"
        },
        "body": "This is a test post made by native android app",
        "body_html": "<p>This is a test post made by native android app</p>\n",
        "comment_count": 1,
        "created_utc": 1599157629,
        "domain": "text post",
        "downvotes": 0,
        "edited_utc": 0,
        "embed_url": "",
        "fullname": "t2_2xv6",
        "guild_name": "RuqqusAPI",
        "id": "2xv6",
        "is_archived": false,
        "is_banned": false,
        "is_deleted": false,
        "is_nsfl": false,
        "is_nsfw": false,
        "original_guild_name": "RuqqusAPI",
        "permalink": "/post/2xv6/native-app-test-post",
        "score": 4,
        "thumb_url": null,
        "title": "Native app test post",
        "upvotes": 4,
        "url": "",
        "voted": 1
    }, {
        "author": "foreverzer0",
        "author_title": {
            "color": "#5555dd",
            "id": 22,
            "kind": 1,
            "text": " the Likeable"
        },
        "body": "I have been working on a Ruby implementation of the API, and am down to the last of the \"common\" functionality, and so far so good, everything works like a charm.\r\n\r\nWhen it comes to implementing [api_vote_post](https://github.com/ruqqus/ruqqus/blob/7dfe5b22732434362a7b98553417d089c3cd0c3b/ruqqus/routes/votes.py#L17) and [api_vote_comment](https://github.com/ruqqus/ruqqus/blob/7dfe5b22732434362a7b98553417d089c3cd0c3b/ruqqus/routes/votes.py#L71), for the life of me I cannot get this to work, and strangest yet it returns a 404, when it clearly exists.\r\n\r\nSo here's what I am doing and what is causing the error. For the sake of example, let's use [this post](https://ruqqus.com/post/1wbo/hi-im-josh-roehl-singer-and) and say I am attempting to upvote it. \r\n\r\n* Have confirmed I am properly authorized, as I can make other API calls both before and after this call fails with the same authentication. I have also confirmed that `vote` is in my scopes.\r\n* `Authorization` header is properly formatted (as I stated, everything else works)\r\n* Build the following URI: https://ruqqus.com/api/v1/vote/post/1wbo/1\r\n* Send an POST request to that URL with no parameters\r\n* 404 error returned\r\n* Retry using the \"full name\" as `t2_1wbo`, same outcome.\r\n* Same thing applies when doing the same with the comment endpoint\r\n\r\nI am at my wit's end, and this simple API call has defeated me. Can anyone even just confirm/deny that this is working for them?\r\n\r\n\r\nEDIT: \r\n\r\nI fixed a typo in a constant that caused the 404, but now I am just back to 401 (Unauthorized), which was the original error for the first 10-20 times I rewrote the method.\r\n",
        "body_html": "<p>I have been working on a Ruby implementation of the API, and am down to the last of the \"common\" functionality, and so far so good, everything works like a charm.</p>\n<p>When it comes to implementing <a href=\"https://github.com/ruqqus/ruqqus/blob/7dfe5b22732434362a7b98553417d089c3cd0c3b/ruqqus/routes/votes.py#L17\" rel=\"nofollow noopener\" target=\"_blank\">api_vote_post</a> and <a href=\"https://github.com/ruqqus/ruqqus/blob/7dfe5b22732434362a7b98553417d089c3cd0c3b/ruqqus/routes/votes.py#L71\" rel=\"nofollow noopener\" target=\"_blank\">api_vote_comment</a>, for the life of me I cannot get this to work, and strangest yet it returns a 404, when it clearly exists.</p>\n<p>So here's what I am doing and what is causing the error. For the sake of example, let's use <a href=\"https://ruqqus.com/post/1wbo/hi-im-josh-roehl-singer-and\">this post</a> and say I am attempting to upvote it.</p>\n<ul>\n<li>Have confirmed I am properly authorized, as I can make other API calls both before and after this call fails with the same authentication. I have also confirmed that <code>vote</code> is in my scopes.</li>\n<li><code>Authorization</code> header is properly formatted (as I stated, everything else works)</li>\n<li>Build the following URI: <a href=\"https://ruqqus.com/api/v1/vote/post/1wbo/1\">https://ruqqus.com/api/v1/vote/post/1wbo/1</a></li>\n<li>Send an POST request to that URL with no parameters</li>\n<li>404 error returned</li>\n<li>Retry using the \"full name\" as <code>t2_1wbo</code>, same outcome.</li>\n<li>Same thing applies when doing the same with the comment endpoint</li>\n</ul>\n<p>I am at my wit's end, and this simple API call has defeated me. Can anyone even just confirm/deny that this is working for them?</p>\n<p>EDIT:</p>\n<p>I fixed a typo in a constant that caused the 404, but now I am just back to 401 (Unauthorized), which was the original error for the first 10-20 times I rewrote the method.</p>\n",
        "comment_count": 4,
        "created_utc": 1599131701,
        "domain": "text post",
        "downvotes": 0,
        "edited_utc": 1599137559,
        "embed_url": "",
        "fullname": "t2_2xgo",
        "guild_name": "RuqqusAPI",
        "id": "2xgo",
        "is_archived": false,
        "is_banned": false,
        "is_deleted": false,
        "is_nsfl": false,
        "is_nsfw": false,
        "original_guild_name": "RuqqusAPI",
        "permalink": "/post/2xgo/is-the-apis-postcomment-voting-broken",
        "score": 6,
        "thumb_url": null,
        "title": "Is the API's post/comment voting broken, or am I just being stupid?",
        "upvotes": 6,
        "url": "",
        "voted": 1
    }, {
        "author": "acikek",
        "author_title": {
            "color": "#aa8855",
            "id": 12,
            "kind": 1,
            "text": ", Guildmaster"
        },
        "body": "If you're reading this, this post was made by a bot!",
        "body_html": "<p>If you're reading this, this post was made by a bot!</p>\n",
        "comment_count": 4,
        "created_utc": 1599076575,
        "domain": "text post",
        "downvotes": 0,
        "edited_utc": 0,
        "embed_url": "",
        "fullname": "t2_2wrn",
        "guild_name": "RuqqusAPI",
        "id": "2wrn",
        "is_archived": false,
        "is_banned": false,
        "is_deleted": false,
        "is_nsfl": false,
        "is_nsfw": false,
        "original_guild_name": "RuqqusAPI",
        "permalink": "/post/2wrn/this-is-a-test-post",
        "score": 6,
        "thumb_url": null,
        "title": "This is a test post!",
        "upvotes": 6,
        "url": "",
        "voted": 1
    }, {
        "author": "Seq37",
        "author_title": {
            "color": "#dd5555",
            "id": 4,
            "kind": 3,
            "text": ", Breaker of Ruqqus"
        },
        "body": "Ruqqus API error codes be like:\r\n\r\n* 401: your token is invalid or expired (\u273f\u25e0\u203f\u25e0)\r\n* 403: you don't have access to this data \u0669\u25d4\u203f\u25d4\u06f6\r\n* 404: this API method does not exist \u2267\u25e1\u2266\r\n* 405: you should probably change your request method \u2256\u203f\u2256\r\n* 500: I\u036f\u0337\u031cn\u036e\u033e\u0352t\u036a\u0369\u0357e\u030d\u0343r\u0350\u036f\u0338n\u0342\u0307\u032ba\u0363\u0314\u033el\u036b\u0351\u0307 \u030f\u0303\u036fS\u0350\u032e\u0332e\u0301\u031a\u0366r\u0314\u036d\u0314v\u0346\u030c\u034ce\u0310\u0335\u0345r\u030f\u0368\u0342 \u036a\u0327\u032aE\u0303\u0327\u033ar\u0304\u0364\u0346r\u034c\u0340\u0354o\u0328\u032e\u0331r\u0346\u0346\u0320",
        "body_html": "<p>Ruqqus API error codes be like:</p>\n<ul>\n<li>401: your token is invalid or expired (\u273f\u25e0\u203f\u25e0)</li>\n<li>403: you don't have access to this data \u0669\u25d4\u203f\u25d4\u06f6</li>\n<li>404: this API method does not exist \u2267\u25e1\u2266</li>\n<li>405: you should probably change your request method \u2256\u203f\u2256</li>\n<li>500: I\u036f\u0337\u031cn\u036e\u033e\u0352t\u036a\u0369\u0357e\u030d\u0343r\u0350\u036f\u0338n\u0342\u0307\u032ba\u0363\u0314\u033el\u036b\u0351\u0307 \u030f\u0303\u036fS\u0350\u032e\u0332e\u0301\u031a\u0366r\u0314\u036d\u0314v\u0346\u030c\u034ce\u0310\u0335\u0345r\u030f\u0368\u0342 \u036a\u0327\u032aE\u0303\u0327\u033ar\u0304\u0364\u0346r\u034c\u0340\u0354o\u0328\u032e\u0331r\u0346\u0346\u0320</li>\n</ul>\n",
        "comment_count": 0,
        "created_utc": 1598950181,
        "domain": "text post",
        "downvotes": 1,
        "edited_utc": 0,
        "embed_url": "",
        "fullname": "t2_2v07",
        "guild_name": "RuqqusAPI",
        "id": "2v07",
        "is_archived": false,
        "is_banned": false,
        "is_deleted": false,
        "is_nsfl": false,
        "is_nsfw": false,
        "original_guild_name": "RuqqusAPI",
        "permalink": "/post/2v07/a-joke-i-came-up-with",
        "score": 9,
        "thumb_url": null,
        "title": "A joke I came up with a while ago",
        "upvotes": 10,
        "url": "",
        "voted": 1
    }]
}
```

###
