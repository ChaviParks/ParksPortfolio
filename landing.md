---
title: Projects
layout: landing
description: A collection of some fun projects<br /> I've created over the years.
image: assets/images/pic07.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

<!-- One -->
<section id="one">
	<div class="inner">
		<p> Below I have created a list of some of the main projects I have worked on during my College Career. Some I have worked on independently, while others were introduced within the classroom. The listing is ordered by recency.</p>
	</div>
</section>

<!-- Two -->
<section id="two">
<div class="spotlights">
	
{% for projects in site.data.myProjects %}
        <section>
        <a href="" class="image">
			<img src="./assets/images/{{ projects.Image }}" alt="" data-position="25% 25%" />
		</a>
    <div class = "content">
    <div class = "inner">
        <header class="major">
        <h3>{{ projects.Project }}</h3>
        <h4>{{ projects.Language }}</h4>
		</header>
     
        <p>{{ projects.Description }}</p>
        </div>
        </div>
        </section>
       {% endfor %}

</div>
</section>	

