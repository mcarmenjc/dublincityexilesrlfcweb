---
title: News
layout: page
---

{% for post in site.posts %}
<div class="card my-3">
    <div class="card-body">
        <h5 class="card-title">{{ post.title}}</h5>
        <p class="dce-post-date">{{ post.date | date: "%b %-d, %Y" }}</p>
        <hr />
        {{ post.content }}
    </div>
</div>
{% endfor %}