---
layout: index
title: Downloads
---
<!-- Main -->
# {{ page.title }}

We have several different formats for you to access our curriculum for your convenience.

## Curriculm

[Microsoft Word Document](barnabasrobotics.com/Barnabas-Bot-Curriculum.docx)  
[Open Document Format](barnabasrobotics.com/Barnabas-Bot-Curriculum.odf) for libreOffice and others  
[PDF](barnabasrobotics.com/Barnabas-Bot-Curriculum.pdf) for Adobe Reader and many other apps  
[EPUB](barnabasrobotics.com/Barnabas-Bot-Curriculum.epub) for use with Google Play Book and Apple Books ([about .epub adoption](https://en.wikipedia.org/wiki/EPUB#Adoption))

## Others

{% for lesson in site.lessons %}
{% for item in lesson.other %}
  - [ {{ item.text }} ]( {{ item.link}} )
{% endfor %}
{% endfor %}
