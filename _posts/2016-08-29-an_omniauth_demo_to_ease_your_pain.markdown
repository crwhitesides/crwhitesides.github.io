---
layout: post
title:  "An Omniauth demo to ease your pain"
date:   2016-08-29 22:29:47 +0000
---

My Omniauth experience (for a while) concluded with this error: `JSON::GeneratorError in Sessions#create`. ((😱 )) The error then specified that "only generation of JSON objects or arrays allowed". Ummmmm, thanks. What does this mean? I still don't know. ((😱 )) However, at this moment, my app allows me to sign in with Facebook, redirects me to my root path (where I am warmly greeted), and includes the ability to log out. Yes, I overcame that error. In fact, I didn't even deal with it. I simply opted to look for a different way to get the same result. It's a beautiful thing, programming. The tests set certain expectations, but the solutions vary. With that said, I give to you the resource that provided me with greater clarity regarding omniauth. Behold, the [Quick Omniauth-Facebook Demo](https://github.com/ralphos/omniauth-facebook-example)!

I hope it helps. ✌🏾
