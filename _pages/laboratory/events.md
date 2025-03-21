---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: page
title: 研究室紹介
permalink: /laboratory/events/
---

## イベント

原則として全員参加の合宿だけでなく，希望者でスポーツ観戦や登山に行くこともあります．以下にこれまでに行ったイベントを挙げておきます．

{% if site.paginate %}
{% assign posts = paginator.events %}
{% else %}
{% assign posts = site.events %}
{% endif %}


{%- if posts.size > 0 -%}
{%- if page.list_title -%}
    <h2 class="post-list-heading">{{ page.list_title }}</h2>
{%- endif -%}
<ul class="post-list">
    {%- assign date_format = site.minima.date_format | default: "%Y/%m/%d" -%}
    {% assign sorted_events = site.events | sort: "path" | reverse %}
  {% for post in sorted_events %}
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
