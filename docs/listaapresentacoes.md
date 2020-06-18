---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Lista de Apresentações
layout: page
show_sidebar: true
---
<ul>
  {% for slide in site.slides %}
    <li>
      <h2><a href="{{site.url}}/{{site.baseurl}}/{{ slide.url }}" target="_blank">{{ slide.title }}</a></h2>
    </li>
  {% endfor %}
</ul>