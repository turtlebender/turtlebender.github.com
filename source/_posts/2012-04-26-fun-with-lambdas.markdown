---
layout: post
title: "Fun with lambdas"
date: 2012-04-26 18:08
comments: true
categories: 
---

Ok, so this is a kinda small thing, but it is a nice little pattern that
I used a lot today while building an oauth 2.0 server for
https://www.globusonline.org  I often need to make sure that a
particular exception was thrown, as part of my "unhappy" testing.  This
is always a little bit of a pain.

``` python test.py 
def test_me(self):
  self.assertRaises(NodeNotFoundException,
     lambda: self.storage.get_node('access_token',
     access_token_data['id']))
``` 

Sticking that lambda in there makes it really easy to check for an
exception.  Groundbreaking?  No.  But very convenient.
