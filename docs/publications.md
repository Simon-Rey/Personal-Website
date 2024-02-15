---
layout: default
title: Publications | Simon Rey
---

# Publications

Here are my publications, I try as much as possible to link each article to an open-source pdf of it.
If something is not available please contact me!

{% assign publications_per_year = site.data.publications | group_by: 'year' %}
{% assign publications_per_year = publications_per_year | sort: 'name' | reverse %}

{% for year_group in publications_per_year %}

<h2 style="text-align: center;">{{ year_group.name }}</h2>

{% for publication in year_group.items %}
<div class="publicationsBox">
<div class="publicationDiams"><strong> &diams; </strong></div>
<div class="publicationText">
<p>
{% for author in publication.authors %}
{% if author.webpage %}
<a href="{{ author.webpage }}" title="Link to {{ author.name }} own webpage">
{% endif %}
{{ author.name }},
{% if author.webpage %}
</a>
{% endif %}
{% endfor %}
<strong>{{ publication.title }}</strong>, {{ publication.published_in }}, {{ publication.year }}.
</p>

{% if publication.comment %}
<p class="publicationComment" style="margin-top: 8px;">
{{ publication.comment }}
</p>
{% endif %}
</div>
<div class="publicationButtons">
{% for link in publication.links %}
<div id="{{ link.type | downcase | replace: ' ', '' }}Button">
<a href="{{ link.url }}" title="Link to the {{ link.type | downcase }} page of the publication">{{ link.type }}</a>
</div>
{% endfor %}
</div>
</div>
{% endfor %}
{% endfor %}
