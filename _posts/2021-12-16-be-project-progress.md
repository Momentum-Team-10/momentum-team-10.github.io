---
layout: post
title: 🐻 API Progress Check-In 🐻
tags: phase-3 phase-3-be admin password
---

## 🗓️ Today's Topics

- How are the projects coming along? 👀

## 🎯 Project

Keep on going. 💪 🚀

We will use class time today to get you past any blockers you may be experiencing and to talk through next steps.

By now you should have provided your front end with a way to log in and log out, and endpoints to see data. By tomorrow you should have the ability to POST data.

## 📖 Read | 📺 Watch | 🎧 Listen

On Monday we'll be covering full-text search in your API, but if you have time you can check these resources out in advance.

- 📖 [Basic and Full-Text Search with Django and Postgres](https://testdriven.io/blog/django-search/)
- 📖 [If you want A LOT more detail about full-text search in Postgres and Django, this blog piece has you covered](https://pganalyze.com/blog/full-text-search-django-postgres)
- 📖 [Blog post with more on full-text search](https://www.netlandish.com/blog/2020/06/22/full-text-search-django-postgresql/)
- [Search from the Ground Up](https://www.youtube.com/watch?v=is3R8d420D4&list=PL2NFhrDSOxgXXUMIGOs8lNe2B-f4pXOX-&index=2) -> DjangoCon 2019 video explaining search in detail


## 🔖 Resources

Make sure you are sharing this information with your front end as well. You can include it in a project README.

- [Base Endpoint Guide for Djoser](https://djoser.readthedocs.io/en/latest/base_endpoints.html) -> includes create a new user and other nice stuff
- [Token Authentication Endpoint Guide for Djoser](https://djoser.readthedocs.io/en/latest/token_endpoints.html) -> details on the token auth endpoints

### Creating a properly hashed password

In order to properly save a hashed password when you create a new user in the Django Admin, make sure you are using `UserAdmin` in `admin.py`:

```py
from django.contrib import admin
from django.contrib.auth.admin import UserAdmin

...

admin.site.register(User, UserAdmin)

```

- [Django Docs: Manually managing a user's password](https://docs.djangoproject.com/en/3.2/topics/auth/passwords/#module-django.contrib.auth.hashers)


## 🦉 Code

- [DRF Library API](https://github.com/Momentum-Team-10/example-drf-library)
