---
layout: index
title: Downloads
---
<!-- Main -->
# {{ page.title }}

We have several different formats for you to access our curriculum for your convenience.

## Barnabas Bot Curriculum Textbook
[Google Doc](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/edit?usp=sharing)  
[Microsoft Word Document](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=docx)  
[Open Document Format](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=odf) for libreOffice and others  
[PDF](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=pdf) for Adobe Reader and many other apps  
[EPUB](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=epub) for use with Google Play Book and Apple Books ([about .epub adoption](https://en.wikipedia.org/wiki/EPUB#Adoption))

## Others
___
<div class="tabs">
	
<div class="tab" id="bot">
<h2><a href="#bot"><i class="icon fa-android"></i> Site Content from Bot Lessons</a></h2>
<div class="content">
	
{% for lesson in site.bot_lessons %}
	
<h4><a href="{{ site.baseurl }}{{ lesson.url }}" target="_balnk">{{ lesson.title }}</a></h4>
{% for item in lesson.videos %}
<a href="{{ item.link}}" target="_balnk">{{ item.text }}</a>
{% endfor %}
{% for item in lesson.documents %}
<a href="{{ item.link}}" target="_balnk">{{ item.text }}</a>
{% endfor %}
{% for item in lesson.other %}
<a href="{{ item.link}}" target="_balnk">{{ item.text }}</a>
{% endfor %}

{% endfor %}

</div>
</div>

<div class="tab" id="racer">
<h2><a href="#racer"><i class="icon fa-car"></i> Site Content from Racer Lessons</a></h2>
<div class="content">

{% for lesson in site.racer_lessons %}

#### [{{ lesson.title }}]({{ site.baseurl }}{{ lesson.url }})
{% for item in lesson.videos %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
{% for item in lesson.documents %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
{% for item in lesson.other %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
    
{% endfor %}

</div>
</div>

</div>
<!-- test setup -->