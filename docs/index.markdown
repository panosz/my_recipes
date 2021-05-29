---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
title: Recipes
---

<ul>
  {% for recipe in site.recipes %}
      <h2>{{ recipe.name }}</h2>
      <h3>{{ recipe.position }}</h3>
      <p>{{ recipe.content | markdownify }}</p>
      <hr>
  {% endfor %}
</ul>
