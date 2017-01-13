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

There's also a [breakdown][1] to serve as a guide as to which chapters should be
included in the [daily reading][1]. Consideration was taken to make sure the
chapters are distributed in such a way that in each day only one book is
covered.

_Ps: Books that I've covered or have began covering should have a link to the
study material. By cover I mean convert to a digital format on the Web — as an
attempt at making my Bible study (which till this point existed mostly in my
head and in notebooks) publicly accessible. Work in progress is marked by a ☆
and complete work by a ★._

_Ps 2: Ultimately, this is intended to be my life's work. It's nowhere near
complete i.e. having content on each book, chapter, [topic][3] and
[character][2]. I figured that I'll never start if choose to start when I know
it all. Feel free to [send comments and feedback][4]. That said, I'll spare you
the scroll down to 1 Kings, Hosea or Philippians._

{% for entry in site.data.breakdown.book_days %}
### {{ entry.section }}

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
      <td>{{ book.title }}</td>
      <td>{{ book.days | join: ' • ' }}</td>
    </tr>
{% endfor %}
  </tbody>
</table>
{% endfor %}

The Protestant Christian Bible has a total of 66 books: 39 in the Old Testament and 27 in the New Testament.

---

1. The main determinant of the number of days allocated to complete a book is
the amount of content i.e. larger books take longer to go through. And by
larger, this isn't referring to the number of chapters but the actual amount of
text in the book.

[1]: {{ site.baseurl }}/about/daily-breakdown/
[2]: {{ site.baseurl }}/people/
[3]: {{ site.baseurl }}/topics/
[4]: mailto:j+st@kingori.co?Subject=Hey%20There...
