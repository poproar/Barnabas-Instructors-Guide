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
<h2><i class="icon fa-android"></i> Site Content from Bot Lessons</h2>

{% for lesson in site.bot_lessons %}

#### [{{ lesson.title }}]({{ site.baseurl }}{{ lesson.url }})
{% for item in lesson.videos %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
{% for item in lesson.documents %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
{% for item in lesson.other %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
    
{% endfor %}
___
<h2><i class="icon fa-car"></i> Site Content from Racer Lessons</h2>

{% for lesson in site.racer_lessons %}

#### [{{ lesson.title }}]({{ site.baseurl }}{{ lesson.url }})
{% for item in lesson.videos %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
{% for item in lesson.documents %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
{% for item in lesson.other %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
    
{% endfor %}

<div class="tabs">
		
    <div class="tab" id="tab1">
        <a href="#tab1">Tab 1</a>
        <div class="content">
            Content of Tab1
        </div>
    </div>

    <div class="tab" id="tab2">
        <a href="#tab2">Tab 2</a>
        <div class="content">
            Content of Tab2
        </div>
    </div>

    <div class="tab" id="tab3">
        <a href="#tab3">Tab 3</a>
        <div class="content">
            Content of Tab3
        </div>
    </div>


</div>
