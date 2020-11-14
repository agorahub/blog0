---
title: muitinⒾ
layout: page
---
{% for category in site.categories %}
  {% if category.first == "initium" %}
  <div>
    {% for post in category.last %}
    <span class="postdate">{{ post.date | preserve_timezones }}</span>
    • <span class="author"><a href="{{site.url}}/{{site.baseurl}}/{{post.categories.first}}_comments/?[{{post.title}}]({{site.url}}{{site.baseurl}}/{{post.url}})"><b>💬</b></a></span>
    {% if post.author != null %} • <span class="author">{{ post.author }}</span> {% endif %}
    <h4><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h4>
    {% endfor %}
  </div>
  {% endif %}the category comments page
{% endfor %}

