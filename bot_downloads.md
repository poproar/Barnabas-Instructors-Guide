---
layout: index
title: Bot Downloads
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

___

## Others

Add new useful links to this section by submitting them to [this page](https://github.com/{{ site.repository }}/edit/master/{{ page.path }}).

<!-- add new links here, copy the line below and remove the comment -->
<!-- [ link_text ]( link_url ){:target="_blank"}   -->
___

## by Lesson
{% for lesson in site.bot_lessons %}

{% if lesson.other.size > 0 or lesson.documents.size > 0 %}
#### [{{ lesson.title }}]({{ site.baseurl }}{{ lesson.url }})
{% for item in lesson.documents %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
{% for item in lesson.other %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
{% endif %}
    
{% endfor %}
___
