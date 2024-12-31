---
layout: layouts/blog.njk
title: "My BLogs"
description: "Update my blog post article content"
pagination:
  data: collections.posts
  size: 6
  reverse: true
testdata:
 - item1
 - item2
 - item3
 - item4
permalink: "blog/{% if pagination.pageNumber > 0 %}page-{{ pagination.pageNumber + 1 }}/{% endif %}index.html"
---
{% include "layouts/blog/blog_list.njk" %}
{% include "layouts/blog/pagination.njk" %}
