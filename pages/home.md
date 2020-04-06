---
layout: layouts/home.njk
title: Home
date: 2016-01-01T00:00:00.000Z
pageTitle: Mabuhay!
---
{% for post in collections.posts %}
    <h2><a href="{{ post.url }}">{{ post.data.pageTitle }}</a></h2>
    <em>{{ post.date | date: "%Y-%m-%d" }}</em>
{% endfor %}