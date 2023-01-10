---
title: Cultural and Historical Context of Site
course: Design Studio
module: Context
staffer_name: Will Martin
youtube_video: YCK_LU0nSnc
course_image: https://uploads-ssl.webflow.com/5ffe375629409928b7986d22/623e44be456d0b83872ad30d_Into_the_Woods_Denver_ScreenCapture.JPG
course_image_alt: A picture of my course.
instructor_name: Will Martin
role: Instructor
email: will@studiobvio.com
website: http://studiobvio.com
pronouns: He/Him
tags:
nav_exclude: true
---

<h2
  class="fs-6 font-weight-bold text-uppercase"
  id="{{ page.title | slugify }}"
>
  {{ page.title }}
</h2>
<div class="staffer">
  <div>
    <h3 class="staffer-name">
      {%- if page.website -%}
      <a href="{{ page.website }}">{{ page.instructor_name }}</a>
      {%- else -%}
      {{ page.instructor_name }}
      {%- endif -%}
      {%- if page.pronouns -%}
      <span class="staffer-pronouns">{{ page.pronouns }}</span>
      {%- endif -%}
    </h3>
    {%- if page.email -%}
    <p><a href="mailto:{{ page.email }}">{{ page.email }}</a></p>
    {%- endif -%}
  </div>
</div>
<img src="{{ page.course_image }}" alt="{{ page.course_image_alt }}" />
<h3>Lecture Video</h3>

{% include youtube.html id="YCK_LU0nSnc" %}

[Link to Lecture Slides](#)
