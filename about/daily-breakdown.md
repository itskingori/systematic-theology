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
### {{ entry.book }}

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

[11]: {{ site.baseurl }}/books/1-kings/

[1-kings]: {{ site.baseurl }}/books/1-kings/
[1-kings-ch1]: {{ site.baseurl }}/books/1-kings/chapter-1/
[1-kings-ch2]: {{ site.baseurl }}/books/1-kings/chapter-2/
[1-kings-ch3]: {{ site.baseurl }}/books/1-kings/chapter-3/
[1-kings-ch4]: {{ site.baseurl }}/books/1-kings/chapter-4/
[1-kings-ch5]: {{ site.baseurl }}/books/1-kings/chapter-5/
[1-kings-ch6]: {{ site.baseurl }}/books/1-kings/chapter-6/
[1-kings-ch7]: {{ site.baseurl }}/books/1-kings/chapter-7/
[1-kings-ch8]: {{ site.baseurl }}/books/1-kings/chapter-8/
[1-kings-ch9]: {{ site.baseurl }}/books/1-kings/chapter-9/
[1-kings-ch10]: {{ site.baseurl }}/books/1-kings/chapter-10/
[1-kings-ch11]: {{ site.baseurl }}/books/1-kings/chapter-11/
[1-kings-ch12]: {{ site.baseurl }}/books/1-kings/chapter-12/
[1-kings-ch13]: {{ site.baseurl }}/books/1-kings/chapter-13/
[1-kings-ch14]: {{ site.baseurl }}/books/1-kings/chapter-14/
[1-kings-ch15]: {{ site.baseurl }}/books/1-kings/chapter-15/
[1-kings-ch16]: {{ site.baseurl }}/books/1-kings/chapter-16/
[1-kings-ch17]: {{ site.baseurl }}/books/1-kings/chapter-17/
[1-kings-ch18]: {{ site.baseurl }}/books/1-kings/chapter-18/
[1-kings-ch19]: {{ site.baseurl }}/books/1-kings/chapter-19/
[1-kings-ch20]: {{ site.baseurl }}/books/1-kings/chapter-20/
[1-kings-ch21]: {{ site.baseurl }}/books/1-kings/chapter-21/
[1-kings-ch22]: {{ site.baseurl }}/books/1-kings/chapter-22/

[hosea]: {{ site.baseurl }}/books/hosea/
[hosea-ch1]: {{ site.baseurl }}/books/hosea/chapter-1/
[hosea-ch2]: {{ site.baseurl }}/books/hosea/chapter-2/
[hosea-ch3]: {{ site.baseurl }}/books/hosea/chapter-3/
[hosea-ch4]: {{ site.baseurl }}/books/hosea/chapter-4/
[hosea-ch5]: {{ site.baseurl }}/books/hosea/chapter-5/
[hosea-ch6]: {{ site.baseurl }}/books/hosea/chapter-6/
[hosea-ch7]: {{ site.baseurl }}/books/hosea/chapter-7/
[hosea-ch8]: {{ site.baseurl }}/books/hosea/chapter-8/
[hosea-ch9]: {{ site.baseurl }}/books/hosea/chapter-9/
[hosea-ch10]: {{ site.baseurl }}/books/hosea/chapter-10/
[hosea-ch11]: {{ site.baseurl }}/books/hosea/chapter-11/
[hosea-ch12]: {{ site.baseurl }}/books/hosea/chapter-12/
[hosea-ch13]: {{ site.baseurl }}/books/hosea/chapter-13/
[hosea-ch14]: {{ site.baseurl }}/books/hosea/chapter-14/

[philippians]: {{ site.baseurl }}/books/philippians/
[philippians-ch1]: {{ site.baseurl }}/books/philippians/chapter-1/
[philippians-ch2]: {{ site.baseurl }}/books/philippians/chapter-2/
[philippians-ch3]: {{ site.baseurl }}/books/philippians/chapter-3/
[philippians-ch4]: {{ site.baseurl }}/books/philippians/chapter-4/
