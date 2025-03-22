---
layout: page
title: 新着情報
permalink: /news/
nav-bar: False
---

{% if site.paginate %}
{% assign posts = paginator.news %}
{% else %}
{% assign posts = site.news %}
{% endif %}


{%- if posts.size > 0 -%}
{%- if page.list_title -%}
    <h2 class="post-list-heading">{{ page.list_title }}</h2>
{%- endif -%}
<ul class="post-list">
    {%- assign date_format = site.minima.date_format | default: "%Y/%m/%d" -%}
    {% assign sorted_news = site.news | sort: "path" | reverse %}
  {% for post in sorted_news %}
    <li>
    <span class="post-meta">{{ post.date | date: date_format }}</span>
    <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
    </a>
    {%- if site.show_excerpts -%}
        {{ post.excerpt }}
    {%- endif -%}
    </li>
    {%- endfor -%}
</ul>

{% if site.paginate %}
    <div class="pager">
    <ul class="pagination">
    {%- if paginator.previous_page %}
        <li><a href="{{ paginator.previous_page_path | relative_url }}" class="previous-page">{{ paginator.previous_page }}</a></li>
    {%- else %}
        <li><div class="pager-edge">•</div></li>
    {%- endif %}
        <li><div class="current-page">{{ paginator.page }}</div></li>
    {%- if paginator.next_page %}
        <li><a href="{{ paginator.next_page_path | relative_url }}" class="next-page">{{ paginator.next_page }}</a></li>
    {%- else %}
        <li><div class="pager-edge">•</div></li>
    {%- endif %}
    </ul>
    </div>
{%- endif %}

{%- endif -%}
