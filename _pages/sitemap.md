---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all the posts and pages found on the site. For you robots out there, there is an [XML version]({{ base_path }}/sitemap.xml) available for digesting as well.


<h2>Pages</h2>
{% for post in site.pages %}
  {% unless post.url contains 'markdown' or post.url contains 'archive-layout' or post.url contains 'non-menu-page' or post.url contains '404' or post.url contains 'terms' or post.url contains 'cv-json' or post.url contains 'sitemap' %}
    {% include archive-single.html %}
  {% endunless %}
{% endfor %}

<h2>Posts</h2>
<!-- {% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %} -->

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
  {% unless collection.output == false or collection.label == "posts" or collection.label == "teaching" or collection.label == "portfolio" %}
  {% capture label %}{{ collection.label }}{% endcapture %}
  {% if label != written_label %}
  <h2>{{ label }}</h2>
  {% capture written_label %}{{ label }}{% endcapture %}
  {% endif %}
{% endunless %}
{% for post in collection.docs %}
  {% unless collection.output == false or collection.label == "posts" %}
  {% include archive-single.html %}
  {% endunless %}
{% endfor %}
{% endfor %}
