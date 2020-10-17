---
title: "Unit Testing .NET Core 3.1 Controllers"
date: 2020-10-17T15:37:43+02:00
draft: true
---

Couple of ways you can unit test your controllers.

# 1. DefaultHttpContext
I have read that its preferred if you just create a new instance of `DefaultHttpContext()` and pass it into your subject controller initialization.

```
var subjectController = new ControllerUnderTest()
{
    HttpContext = new DefaultHttpContext()
}
```

Also note that this is the best 
# Method number 2
This is also number