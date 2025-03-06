---
layout: default
title: Simon Rey
main_style: "padding: 0;"
---

<div id="newsbox">
<div id ="newscontent" style="line-height: 1.5; text-align: justify;" markdown="1">

# Presentation

I used to be an academic researching questions related to the aggregation of preferences for collective decision-making.
I have now changed to a completely different path, but will maintain this website for legacy purposes.

In my last academic position, I worked a senior scientific programmer in the Collective Information project of 
[Ulle Endriss](https://staff.science.uva.nl/u.endriss/ "Link to Ulle Endriss's personal page")
at the [Institute for Logic, Language and Computation (ILLC)](http://illc.uva.nl "Link to the ILLC main page")
at the University of Amsterdam located (surprisingly) in Amsterdam, The Netherlands.

Before that, I did my PhD under the supervision of 
[Ulle Endriss](https://staff.science.uva.nl/u.endriss/ "Link to Ulle Endriss's personal page"), 
[Jan Maly](https://janmaly.de/ "Link to Jan Maly's personal page"), and
[Ronald de Haan](https://staff.science.uva.nl/r.dehaan/ "Link to Ronald de Haan's personal page").
My thesis titled [Variations on Participatory Budgeting](/static/publications/Rey23.pdf) presents a wide range of approaches I used to analyse participatory budgeting.

The field I worked in is called as 
[Computational Social Choice](https://comsoc-community.org "Link to the Computational Social Choice websute").
The typical problems arising in (computational) social choice concern the aggregation of individual
opinions into a collective, such as when people vote in an election. I studied different questions 
related to the aggregation of preferences, both from a mathematical and from a computational perspective.

I mostly focused on participatory budgeting, a democratic tool used to allow citizens to vote on how
to allocation public funds. I have also worked on other topics such as the fair allocation of
indivisible items, or how to handle incomplete preferences. I developed several tools during my time 
as a researcher: I was the main developer and maintainer of [PrefLib.org](https://www.preflib.org/), 
the [PaBuTools](https://pypi.org/project/pabutools/), among others.

If you have no idea what social choice scientists do, the following video will offer you a glimpse
at the typical problems we study when it comes to participatory budgeting.

<div class="videoWrapper">
<iframe width="560" height="315" src="https://www.youtube.com/embed/iSX90xJjSAw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
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