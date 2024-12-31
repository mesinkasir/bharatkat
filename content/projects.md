---
layout: layouts/themes.njk
title: "My Projects"
description: "My Projects for 11ty eleventy , Astro Js, Jekyll , Angular, Svelte, Gatsby Js, Next Js , Docusaurus, Starlight Js, and Others"
pagination:
  data: collections.ourprojects
  size: 6
  reverse: true
testdata:
 - item1
 - item2
 - item3
 - item4
permalink: "projects/{% if pagination.pageNumber > 0 %}page-{{ pagination.pageNumber + 1 }}/{% endif %}index.html"
---
{% include "layouts/theme/theme_list.njk" %}
{% include "layouts/theme/pagination.njk" %}
