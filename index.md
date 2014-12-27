---
layout: page
title: Avolt Pages
---
{% include JB/setup %}

<ul class="posts">
    {% for post in site.posts %}
    <li>
        <span>{{ post.date | date_to_string }}</span> 
        - <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endfor %}

{% highlight ruby %}
desc "Launch preview environment"
task :preview do
system "jekyll --auto --server"
end # task :preview
{% endhighlight %}

</ul>