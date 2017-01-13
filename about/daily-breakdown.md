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
      <td>{{ day.count }}</td>
      <td>{{ day.chapters | join: ' • ' }}</td>
    </tr>

  {% endfor %}
  </tbody>
</table>

{% endfor %}

[1]: {{ site.baseurl }}/
