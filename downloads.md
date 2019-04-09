---
layout: index
title: Downloads
---
<!-- Main -->
# {{ page.title }}

We have several different formats for you to access our curriculum for your convenience.

## Barnabas Bot Curriculum
[Google Doc](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/edit?usp=sharing)  
[Microsoft Word Document](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=docx)  
[Open Document Format](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=odf) for libreOffice and others  
[PDF](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=pdf) for Adobe Reader and many other apps  
[EPUB](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=epub) for use with Google Play Book and Apple Books ([about .epub adoption](https://en.wikipedia.org/wiki/EPUB#Adoption))

## Others
<h3><i class="icon fa-android"></i>Site Content from Bot Lessons</h3>
<ul>
    {% for lesson in site.bot_lessons %}
    <li><a href="{{ site.baseurl }}{{ lesson.url }}">{{ lesson.title }}</a></li>
        <ul>
             {% for item in lesson.videos %}
            - [ {{ item.text }} ]( {{ item.link}} )  
            {% endfor %}
            {% for item in lesson.documents %}
            - [ {{ item.text }} ]( {{ item.link}} )  
            {% endfor %}
             {% for item in lesson.other %}
            - [ {{ item.text }} ]( {{ item.link}} )  
            {% endfor %}
        </ul>
    {% endfor %}
</ul>

<h3><i class="icon fa-android"></i>Additional Content for Bot Lessons</h3>
<ul>
    <li><a href="https://linkurl">Link Name</a></li>
</ul>

<h3><i class="icon fa-car"></i>Site Content from Racer Lessons</h3>
<ul>
    {% for lesson in site.racer_lessons %}
    <li><a href="{{ site.baseurl }}{{ lesson.url }}">{{ lesson.title }}</a></li>
        <ul>
             {% for item in lesson.videos %}
            - [ {{ item.text }} ]( {{ item.link}} )  
            {% endfor %}
            {% for item in lesson.documents %}
            - [ {{ item.text }} ]( {{ item.link}} )  
            {% endfor %}
             {% for item in lesson.other %}
            - [ {{ item.text }} ]( {{ item.link}} )  
            {% endfor %}
        </ul>
    {% endfor %}
</ul>

<h3><i class="icon fa-checkered-flag"></i>{{ site.racer_lessons.links.title }}</h3>

{% for item in site.racer_lessons.links.items %}
- [ {{ item.text }} ]( {{ item.link}} )  
{% endfor %}