---
layout: default
title: Get a random photo
anchor: get-a-random-photo
front: false
permalink: /photos/getrandom
---

## Get a random photo


```
GET /random
```

### Parameters

None

### Response

```javascript
200 OK
X-Ratelimit-Limit: 1000
X-Ratelimit-Remaining: 999
```


> *Note:* To access a user’s private data, the user is required to authorize the read_user scope. Without it, this request will return a 403 Forbidden response.

