---
layout: default
title: Talks | Simon Rey
---

# Talks

Here are few talks I've given, the slides may not be up to date! If you have any questions, do contact me.

{% for talk in site.data.talks %}
<div class="talkBox">
<h2>{{ talk.title | safe }} <br>
{% if talk.venueURL %}
<a href="{{ talk.venueURL }}">{{ talk.event }}</a> -
{% else %}
{{ talk.event }} -
{% endif %}
{{ talk.date }}</h2>
<table>
<tr>
<td style="padding-right: 20px">
<p>{{ talk.description | safe }}</p>
</td>
<td style="width: 10ch;">
{% if talk.pdf_file %}
<span class="pdfButton">
<a href="{{ talk.pdf_file }}" title="Link to the PDF file of the talk">PDF File</a>
</span>
{% endif %}
</td>
</tr>
</table>
</div>
{% endfor %}
