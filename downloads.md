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

<ul class="nav nav-tabs">
    <li class="active"><a data-toggle="tab" href="#home">Home</a></li>
    <li><a data-toggle="tab" href="#menu1">Menu 1</a></li>
    <li><a data-toggle="tab" href="#menu2">Menu 2</a></li>
    <li><a data-toggle="tab" href="#menu3">Menu 3</a></li>
  </ul>

  <div class="tab-content">
    <div id="home" class="tab-pane fade in active">
      <h3>HOME</h3>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
    </div>
    <div id="menu1" class="tab-pane fade">
      <h3>Menu 1</h3>
      <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
    </div>
    <div id="menu2" class="tab-pane fade">
      <h3>Menu 2</h3>
      <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam.</p>
    </div>
    <div id="menu3" class="tab-pane fade">
      <h3>Menu 3</h3>
      <p>Eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p>
    </div>
  </div>
