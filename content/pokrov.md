---
data: collections
layout: layouts/home.njk
title: Покровський район. Гуманітарні центри
description: This is a post on My Blog about leveraging agile frameworks.
---

<h1>Tagged “{{ tag }}”</h1>

{% set postslist = collections[ tag ] %}
{% include "postslist.njk" %}

<p>See <a href="/tags/">all tags</a>.</p>