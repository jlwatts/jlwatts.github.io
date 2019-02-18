---
layout: page
permalink: /categories/tech
title: tech
---
{% for post in site.categories[page.title] %}
<div class="post">
    <h1 class="post-title">
      <a href="{{ site.baseurl }}/{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>

    <span class="post-date">{{ post.date | date_to_string }}</span>

    {{ post.excerpt }}
    
    <a class="post-expand" href="{{ site.baseurl }}{{ post.url }}">~ Read more ~</a>

  </div>
{% endfor %}