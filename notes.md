---
layout: page
title: 筆記
permalink: /notes/
---
## Swift
{% for note in site.swift-notes %} 
  [{{ note.title }}]({{ note.url }})
{% endfor %}
