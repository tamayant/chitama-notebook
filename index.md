---
layout: default
title: ちーたまノート
---

## ここはちーとたまやんの「菜園・料理・技術」のノートです🌱

<h3>記事一覧</h3>
<ul>
  {% for post in site.posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

<h3>カテゴリ一覧</h3>
<ul>
  {% for category in site.categories %}
    {% assign name = category[0] %}
    <li>
      <a href="/category/{{ name | uri_escape }}/">
        {{ name }}（{{ category[1].size }}記事）
      </a>
    </li>
  {% endfor %}
</ul>