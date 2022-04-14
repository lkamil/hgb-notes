---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
# Index

## Sommersemester 2022
- Klassentreffen Grundstudium Medienkunst

<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>

    <div class="category-head"><b>{{ category_name }}</b></div>
    <a name="{{ category_name | slugize }}"></a>
    <ul>
        {% for post in site.categories[category_name] %}
        <article class="archive-item">
        <li><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></li>
        </article>
        {% endfor %}
    </ul>
  </div>
{% endfor %}
</div>
