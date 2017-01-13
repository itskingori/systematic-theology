---
title: Daily Breakdown
layout: daily-breakdown
permalink: /about/daily-breakdown/
---

This [study plan][1] is designed to cover the entire Bible in 364 days
(approximately 1 year). The amount of text i.e. number of pages of the book is
taken into account so as to fairly distribute the amount of time required to
cover any particular book. This means that longer books will require more days
to go through.

The schedule below details the chapters to cover per day.

{% for entry in site.data.breakdown.day_chapters %}
<h3>{{ entry.book }}</h3>

<table>
  <thead>
    <tr>
      <th>Day</th>
      <th>Content to cover</th>
    </tr>
  </thead>
  <tbody>
  {% for day in entry.days %}

    <tr>
      {% assign slug = entry.book | replace: ' ', '-' | downcase %}
      {% assign book_url = 'https://enduringword.com/commentary/' | append: slug %}
      <td>{{ day.count }}</td>
      <td>
        {% for chapter in day.chapters %}
          {% if slug == 'proverbs' or slug == 'lamentations' or slug == 'ezra' %}
            Chapter {{ chapter }} •
          {% else %}
            {% assign chapter_url = book_url | append: '-' | append: chapter %}
            <a target="_blank" href="{{ chapter_url }}">Chapter {{ chapter }} •</a>
          {% endif %}
        {% endfor %}
      </td>
    </tr>

  {% endfor %}
  </tbody>
</table>

{% endfor %}

[1]: {{ site.baseurl }}/
