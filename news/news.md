---
layout: page
title: 新着情報
permalink: /news
---

# 新着情報

<table class="news">
    <tbody>
        {% for post in site.posts%}
        <tr>
        {% assign date_format = site.minima.date_format | default: "%Y/%m/%d" %}
        <th>{{ post.date | date: date_format }}</th>
        <td><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></td>
        </tr>
        {% endfor %}
    </tbody>
</table>
