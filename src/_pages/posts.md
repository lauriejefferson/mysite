---
layout: page
title: Posts
---

<ul>
  {% for post in collections.posts.resources %}
    <li>
        <a href="{{ post.relative_url }}">{{ post.data.title }}</a>
        <div class="tags">
          {% for tag in post.data.tags %}
            <small>{{ tag }}</small>
          {% endfor %}
        </div>
    </li>
  {% endfor %}
</ul>

If you have a lot of posts, you may want to consider adding [pagination](https://www.bridgetownrb.com/docs/content/pagination)!
