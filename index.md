---
layout: page
title: Avolt Pages
img : https://lh3.googleusercontent.com/-gqTSU8rTpDE/VKOOxOqSBdI/AAAAAAAAAGk/ubQv9tIijTU/w1024-h335-no/avoltpages.jpg

---
{% include JB/setup %}


<ul class="posts">
    {% for post in site.posts %}
    <li>
        <span>{{ post.date | date_to_string }}</span> 
        - <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endfor %}
</ul>