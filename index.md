---
title: King'ori's
layout: index
permalink: /
description: |-
  Daily collection and exploration of the God's authoritative Word which we
  should study because 'All scripture is given by inspiration of God, and is
  profitable for doctrine, for reproof, for correction, for instruction in
  righteousness (2 Timothy 3:16 - KJV).
---

The Bible is God's authoritative Word which [covers several topics][3] and
involves [different people with diverse backgrounds, characters and
abilites][2]. We should not only read through it but study it deeply ... in this
marvelous story **Jesus Christ is the centerpiece!**

This study plan is designed to cover the entire Bible in 364 days (approximately
1 year). The amount of text i.e. number of pages of the book is taken into
account so as to fairly distribute the amount of time required to cover any
particular book. This means that longer books will require more days to go
through.

There's also a [breakdown to serve as a guide as to which chapters should be
included in the daily reading][1]. Consideration was taken to make sure the
chapters are distributed in such a way that in each day only one book is
covered.

{% for entry in site.data.breakdown.book_days %}
<h3>{{ entry.section }}</h3>

<table>
  <thead>
    <tr>
      <th>Book</th>
      <th>Day of the Year</th>
    </tr>
  </thead>
  <tbody>
  {% for book in entry.books %}

    <tr>
    {% assign slug = book.title | replace: ' ', '-' | downcase %}

    {% if slug == 'proverbs' or slug == 'lamentations' or slug == 'ezra' %}
      <td>{{ book.title }}</td>
      <td>{{ book.days | join: ' • ' }}</td>
    {% else %}
      {% assign book_url = 'https://enduringword.com/commentary/' | append: slug | append: '-1' %}
      <td><a target="_blank" href="{{ book_url }}">{{ book.title }}</a></td>
      <td><a target="_blank" href="{{ book_url }}">{{ book.days | join: ' • ' }}</a></td>
    {% endif %}
    </tr>

  {% endfor %}
  </tbody>
</table>
{% endfor %}

The Protestant Christian Bible has a total of 66 books: 39 in the Old Testament
and 27 in the New Testament.

---

1. The main determinant of the number of days allocated to complete a book is
   the amount of content i.e. larger books take longer to go through. And by
   larger, this isn't referring to the number of chapters but the actual amount
   of text in the book.

[1]: {{ site.baseurl }}/about/daily-breakdown/
[2]: {{ site.baseurl }}/people/
[3]: {{ site.baseurl }}/topics/
[4]: mailto:j+st@kingori.co?Subject=Hey%20There...
