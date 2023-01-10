---
layout: page
title: Facilitators
description: A listing of all the ABC School facilitators.
---

# ABC School Facilitators

Staff information is stored in the `_staffers` directory and rendered according to the layout file, `_layouts/staffer.html`.

## Facilitators

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

## Organizers

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
