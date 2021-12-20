---
layout: post
title: 🐻 Search & Automatic Deploys 🐻
tags: phase-3 phase-3-be full-text-search deploy file-upload
---

## Today's Topics

- Postgres full-text search
- Automatic deploys with Heroku's GitHub integration

## 🎯 Project due on Wednesday afternoon

👉 If your project meets minimum requirements today, HUZZAH! That is awesome. You should be working on **at least one spicy feature**.

👉 If your project does not yet meet minimum requirements, you should shoot for meeting them **by the end of the day tomorrow**.

### Note

Depending on how you've constructed your API, you might have separate endpoints for all of the below, or you might have fewer endpoints (for instance, if you nested answers in the question detail endpoint). What matters is that you have endpoints your front-end team can use to access this data, and they are documented somewhere.

### QuestionBox, Back End

- login, logout, and register
- list all questions and answers
- create a question
- create an answer
- mark an answer to own question as "accepted"
- list of all questions and all answers for an authenticated user
- star/favorite questions or answers

### Social Cards, Back End

- login, logout, and register
- list all cards
- list all cards for a user you follow
- list all cards for an authenticated user
- create a new card
- follow/unfollow another user
- list all users an authenticated user follows

## 📖 Read | 📺 Watch | 🎧 Listen

- 📖 [Basic and Full-Text Search with Django and Postgres](https://testdriven.io/blog/django-search/)
- 📖 [If you want A LOT more detail about full-text search in Postgres and Django, this blog piece has you covered](https://pganalyze.com/blog/full-text-search-django-postgres)
- 📖 [Blog post with more on full-text search](https://www.netlandish.com/blog/2020/06/22/full-text-search-django-postgresql/)
- 📺 [Search from the Ground Up](https://www.youtube.com/watch?v=is3R8d420D4&list=PL2NFhrDSOxgXXUMIGOs8lNe2B-f4pXOX-&index=2) -> DjangoCon 2019 video explaining search in detail
- 📺 [Pretty Printed: How to Perform Full Text Searches in Django with Postgres](https://www.youtube.com/watch?app=desktop&v=139a0fm0YFY)


## 🔖 Resources

### `@action` decorator in ViewSets

- [DRF Docs: Marking extra actions for routing with the `@action` decorator](https://www.django-rest-framework.org/api-guide/viewsets/#marking-extra-actions-for-routing)
- [DRF Docs: Routing for extra actions](https://www.django-rest-framework.org/api-guide/routers/#routing-for-extra-actions)

### Filtering and search

- [DRF - Filtering](https://www.django-rest-framework.org/api-guide/filtering/) -> Pretty useful reference. Includes how to filter your output based on GET parameters, which you will want to do for using search terms.
- [Django Docs: full-text search & the search lookup](https://docs.djangoproject.com/en/3.2/ref/contrib/postgres/search/#the-search-lookup)
- [Django Docs: SearchVector](https://docs.djangoproject.com/en/3.2/ref/contrib/postgres/search/#searchvector) -> You'll need this if you want to search against more than a single field

## 🦉 Code & Notes

- [DRF Library API](https://github.com/Momentum-Team-10/example-drf-library)
- [Notes on Django Queries](https://github.com/Momentum-Team-10/notes/blob/main/django-queries.md) These are the same notes you may have seen at the beginning of the Phase. I'm including them here for easy reference, as they show examples of queries and filters that might come in handy for search endpoints.
