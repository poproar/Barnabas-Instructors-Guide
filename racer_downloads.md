---
layout: index
title: Racer Downloads
---
<!-- Main -->
# {{ page.title }}

Our Racer program is a work in progress.

___

## Others

Add new useful links to this section by submitting them to [this page](https://github.com/{{ site.repository }}/edit/master/{{ page.path }})

<!-- add new links here, copy the line below and remove the comment -->
<!-- [ link_text ]( link_url ){:target="_blank"}   -->
[Sal Castro 2019](https://drive.google.com/drive/folders/1dXXoinYFF0HG3lBjUSJnrHYt0mPk1r6G)

___

## by Lesson
{% for lesson in site.racer_lessons %}

{% if lesson.other.size > 0 or lesson.documents.size > 0 %}
#### [{{ lesson.title }}]({{ site.baseurl }}{{ lesson.url }})
{% for item in lesson.documents %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
{% for item in lesson.other %} [ {{ item.text }} ]( {{ item.link}} ){:target="_blank"}  
{% endfor %}
{% endif %}
    
{% endfor %}
___