---
layout: page-fullwidth
permalink: /publication/
title: "Publications"
---
<!-- This page is automatically generated using entries from the file "_data/publications.yml" 
     Please use the file "_data/publications.yml" to include new items.

     Supported classes are:
       "peer-reviewed": Peer-Reviewed Journal Articles
       "under-review": Under Review
       "thesis": PhD Thesis
       "dissertation": Master Dissertation
-->

<!-- To change the list layout go to "_sass/_09_elements.scss 
     under the /* Publication list style */ header  (.publication css class)
-->

## Peer-Reviewed Journal Articles

<!-- Automatically imports class "peer-reviewed" items from file _data/publications.yml -->
<ul class="publication">
  {% for publication_item in site.data.publications %}
  {% if publication_item.class == "peer-reviewed" %}
    <li> {{ publication_item.authors }} ({{ publication_item.year }})
    <a href="{{ publication_item.doi }}">{{ publication_item.title }}</a>.
    <i>{{ publication_item.journal }}</i>
    {{ publication_item.volume }}{% if publication_item.number %}({{ publication_item.number }}){% endif %}: {{ publication_item.pages }}.
    </li>
  {% endif %}
  {% endfor %}
</ul>
{% include _small-top-button.html %}

## Under Review

<!-- Automatically imports class "under-review" items from file _data/publications.yml -->
<ul class="publication">
  {% for publication_item in site.data.publications %}
  {% if publication_item.class == "under-review" %}
    <li> {{ publication_item.authors }} ({{ publication_item.year }})
    <a href="{{ publication_item.doi }}">{{ publication_item.title }}</a>.
    <i>{{ publication_item.journal }}</i>.
    </li>
  {% endif %}
  {% endfor %}
</ul>
{% include _small-top-button.html %}

## PhD Thesis

<!-- Automatically imports class "thesis" items from file _data/publications.yml -->
<ul class="publication">
  {% for publication_item in site.data.publications %}
  {% if publication_item.class == "thesis" %}
    <li> {{ publication_item.authors }} ({{ publication_item.year }})
    <a href="{{ publication_item.doi }}">{{ publication_item.title }}</a>.
    <i>{{ publication_item.institution }}</i>, {{ publication_item.address }}.
    </li>
  {% endif %}
  {% endfor %}
</ul>
{% include _small-top-button.html %}

## Master Dissertation

<!-- Automatically imports class "dissertation" items from file _data/publications.yml -->
<ul class="publication">
  {% for publication_item in site.data.publications %}
  {% if publication_item.class == "dissertation" %}
    <li> {{ publication_item.authors }} ({{ publication_item.year }})
    <a href="{{ publication_item.doi }}">{{ publication_item.title }}</a>.
    <i>{{ publication_item.institution }}</i>, {{ publication_item.address }}.
    </li>
  {% endif %}
  {% endfor %}
</ul>
