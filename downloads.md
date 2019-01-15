---
layout: index
title: Downloads
---
<!-- Main -->
# {{ page.title }}

We have several different formats for you to access our curriculum for your convenience.

## Curriculum
[Google Doc](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/edit?usp=sharing)  
[Microsoft Word Document](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=docx)  
[Open Document Format](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=odf) for libreOffice and others  
[PDF](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=pdf) for Adobe Reader and many other apps  
[EPUB](https://docs.google.com/document/d/13SxcQZP4Q4WikH01lJvGHbPfcNjATRUS2-nPwks0Yi0/export?format=epub) for use with Google Play Book and Apple Books ([about .epub adoption](https://en.wikipedia.org/wiki/EPUB#Adoption))

## Others

{% for lesson in site.lessons %}
{% for item in lesson.other %}
[ {{ item.text }} ]( {{ item.link}} )  
{% endfor %}
{% endfor %}
