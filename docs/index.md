---
layout: default
title: Simon Rey
main_style: "padding: 0;"
---

<div id="newsbox">
<div id ="newscontent" style="line-height: 1.5; text-align: justify;" markdown="1">

Simon Rey here, a multifaceted individual who is always happy to explore new aspects of life. Some of them:

<div id="life-aspects-list">
<div class="life-aspect-header">Woodworking</div><div class="life-aspect-text">I currently work as a furniture maker at <a href="https://reifier.nl" alt="Link to Réifier, furniture making company in Amsterdam.">Réifier</a>, reach out if you're looking for custom shelves.</div>
<div class="life-aspect-header">Programming</div><div class="life-aspect-text"> I also sell my services as freelance programmer with a special interest for theoretic computer science related-projects. Do you have a cool idea for an outreach website but don't have the time to develop it? Reach out, I'll happily do it for you.</div>
<div class="life-aspect-header">Academia</div><div class="life-aspect-text"> I used to be an academic researching questions related to the aggregation of preferences for collective decision-making. You can find all about it on this website.</div>
<div class="life-aspect-header">Photography</div><div class="life-aspect-text"> I love to explore the artistic side of life, through the design of furniture, but also through the <a href="https://photos.simonrey.fr" alt="Link to the photo website of Simon Rey">lens of my cameras</a>.</div>
<div class="life-aspect-header">Consumerism</div><div class="life-aspect-text"> Ever been curious about what you consume and how worth it is each item you buy? I am, check this out at the <a href="https://petitbonhomme.eu/" alt="Link to the website Petit Bonhomme Simon.">Petit Bonhomme Simon</a>.</div>
</div>

</div>

<div id="newscol">
<h2 style="text-align: center;">News</h2>

{% assign sorted_new = site.data.news | sort:"publication_date" | reverse %}
{% for news in sorted_new %}

<div id="news">
<h3> {{ news.title }} </h3>
<p>	{{ news.text | safe }} </p>
</div> 
{% endfor %}
<div id="news"></div>
</div>