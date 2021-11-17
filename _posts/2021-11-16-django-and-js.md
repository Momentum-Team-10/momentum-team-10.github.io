---
layout: post
title: 🍔 Django with a Side of JavaScript 🍟
tags: phase-2 django javascript ajax search
---

## 🗓️ Today's Topics

- Progress report on Code Snippets and Flashcards
- Incorporating JavaScript in a Django application

## 🎯 Project: Code Snippets | Flashcards

Still working on your project. (っ^з^)♪♬

#### Where you should be with Flashcards today

A logged in user should be able to see a list of all the decks, see the cards in a given deck (after it is selected from the list, for instance), and see the question and answer on a given card. The forms for creating a deck and creating cards for a deck should be done by now. You should be working on marking a card as answered, correctly or incorrectly, and be able to record that data somewhere. If decks belong to one user and are not shared, then you could record this on your deck, but it's up to you how you model this.

#### Where you should be with Code Snippets today

A logged in user should be able to see a list of all public snippets and a list of their own snippets, to create new snippets, and to edit and delete existing snippets. You should have a way to manage copying snippets on the back end at least. You may also be ready to start implementing syntax highlighting with JS by this afternoon or evening.

## 🔖 Resources

### Debugging while you work

Setting a breakpoint can help you figure out what code you need in your views!

- [Python debugger commands](https://docs.python.org/3/library/pdb.html?highlight=debugger#debugger-commands)
- [Django Debug Toolbar docs](https://django-debug-toolbar.readthedocs.io/en/latest/)

### JavaScript & Django

- [Django and AJAX](https://realpython.com/django-and-ajax-form-submissions/)
- [Fetching Data with Ajax and Django](https://www.brennantymrak.com/articles/fetching-data-with-ajax-and-django.html) -> This article is really helpful and has really good code examples. Important notes:
  > By including the 'X-Requested-With' header set to 'XMLHttpRequest' [in the AJAX request], the view will be able to check if the request is AJAX or not.

{% highlight python %}
    # In the view function that handles the AJAX request
    request.headers.get('x-requested-with') == 'XMLHttpRequest'
{% endhighlight %}

- [Django docs on the above](https://docs.djangoproject.com/en/3.2/ref/request-response/#django.http.HttpRequest.is_ajax)
- [Working with AJAX in Django](https://testdriven.io/blog/django-ajax-xhr/)
- [MDN: Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) _Remember JS? 🥴 Here's a refresher on using Fetch._
- [Django CSRF with AJAX](https://docs.djangoproject.com/en/3.2/ref/csrf/#ajax)

## ⭐ EXTRA/TMI

- [Django Views the Right Way](https://spookylukey.github.io/django-views-the-right-way/the-pattern.html) _This is a detailed, informative deep dive on function-based views in Django and the reasons why, in the author's opinion, they are better than class-based views._
- [jQuery](https://jquery.com/) _This is not something I recommend using right now, but I include it here because a lot of the resources about using JavaScript in a web browser refer to it (several of the articles above do). It is not as popular as it once was, and it is incompatible with a framework like React. But you will sometimes come across it, and you may end up working with it at your job, so you might as well recognize it when you see it and look it up if you ever need it._

## 🦉 Code

- [Django Music: Basic Search example](https://github.com/Momentum-Team-10/example-django-music/commit/abc285ae36e0cf6a3e64ea5df88fa73ff7d3d6b6)
- [Django Music: More Search examples](https://github.com/Momentum-Team-10/example-django-music/commit/4a5c94feb3c9fb7231bf8e8e866fd1af9f17848f)
- [Django Music: Adding JS](https://github.com/Momentum-Team-10/example-django-music/commit/cc93a888dc7c1cf5f80d87c960662f6190964f05)
