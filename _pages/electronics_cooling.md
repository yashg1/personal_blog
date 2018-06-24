---
layout: archive
permalink: /pcm_elec_cooling/
title: "Cooling Smartphones using Phase Change Materials"
author_profile: true
---

{% include base_path %}
{% include group-by-array collection=site.posts field="tags" %}

{% for tag in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ tag | slugify }}" class="archive__subtitle">{{ tag }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}

{% include figure image_path="https://mmistakes.github.io/minimal-mistakes/assets/images/unsplash-image-10.jpg" alt="this is a placeholder image" caption="This is a figure caption." %}
