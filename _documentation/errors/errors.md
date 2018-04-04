---
layout: default
title: Errors
front: true
order: 3
permalink: /errors/
---

-------------------
# {{page.title}}

If an error occurs, whether on the server or client side, the error message(s) will be returned in an errors array. For example:

```javascript
422 Unprocessable Entity
```

```json
{
  "errors": ["Username is missing", "Password cannot be blank"]
}
```