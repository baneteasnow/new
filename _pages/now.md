---
# {{ 200 | times: 5 | divided_by: 100 }}
# {% include postcountbymonth.html %}
# Here's a sentence with a footnote. [^aaa]
# [^aaa]: This is the footnote.
# term
# : definition
#
# format: book, ebook, audiobook
read: 4
#
layout: page
title: şimdi okuduğum kitaplar
last_modified_at: 2025-01-12
published: true
#
# 1
booktitle1: "Stuff Every Coffee Lover Should Know"
bookyear1: 2024
author1: "Candace Rose Rardon"
sayfa1: 184
format1: reading as a book
pageread1: 34
#
# 2
booktitle2: "Ultra-Processed People - The Science Behind Food That Isn't Food"
bookyear2: 2024
author2: "Chris van Tulleken"
sayfa2: 432
format2: reading as a book
pageread2: 20
#
# 3
booktitle3: "Empire of Pain"
bookyear3: 2024
author3: "Patrick Radden Keefe"
sayfa3: 632
format3: reading as an ebook
pageread3: 30
#
# 4
booktitle4: "The DNA Field and the Law of Resonance"
bookyear4: 2019
author4: "Pierre Franckh"
suresaat4: 4
suredakika4: 45
sayfa4: 285
format4: listening as an audiobook
pageread4: 22
pagereadsaat4: 0
pagereaddakika4: 22
#
#
# ⁜ {{ page.read | plus: 2 }}
#
# {{ page.booktitle2 }} ({{ page.bookyear2 }})
# _by_ {{ page.author2 }}
#
# <div style="font-size: 50%; font-style: italic;">
#   {{ page.sayfa2 }} sayfa
#  </div>
#
# <div style="font-size: 50%; font-style: italic;" title="reading challenge 2025">
#   {{ page.pageread2 | times: 100 | divided_by: page.sayfa2 }}%
# </div>
#
# <div>
#   <progress title="{{ page.pageread2 }}/{{ page.sayfa2 }}" value="{{ page.pageread2 }}" max="{{ page.sayfa2 }}" style="width: 80%;"></progress>
#   <span style="font-size: 50%; font-style: italic;" title="reading challenge 2025">
#     {{ page.pageread2 }}/{{ page.sayfa2 }}
#   </span>
# </div>
# <div style="clear: both"></div>
# <br />
#
#
---

{% include image-gallery.html folder="/assets/now" %}

<div style="clear: both"></div>

⁜ {{ page.read | plus: 1 }}

{{ page.booktitle1 }} ({{ page.bookyear1 }})  
_by_ {{ page.author1 }}

<div style="font-size: 50%; font-style: italic;"> {{ page.format1 }} </div>

  <div style="font-size: 50%; font-style: italic;">
   {{ page.sayfa1 }} sayfa
 </div>

 <div style="font-size: 50%; font-style: italic;" title="reading challenge 2025"> 
   {{ page.pageread1 | times: 100 | divided_by: page.sayfa1 }}%
 </div>

 <div>
   <progress title="{{ page.pageread1 }}/{{ page.sayfa1 }}" value="{{ page.pageread1 }}" max="{{ page.sayfa1 }}" style="width: 80%;"></progress>
   <span style="font-size: 50%; font-style: italic;" title="reading challenge 2025"> 
     {{ page.pageread1 }}/{{ page.sayfa1 }}
   </span>
 </div>

<br />
<div style="clear: both"></div>

⁜ {{ page.read | plus: 2 }}

{{ page.booktitle2 }} ({{ page.bookyear2 }})  
_by_ {{ page.author2 }}

<div style="font-size: 50%; font-style: italic;"> {{ page.format2 }} </div>

  <div style="font-size: 50%; font-style: italic;">
  {{ page.sayfa2 }} sayfa
  </div>

  <div style="font-size: 50%; font-style: italic;" title="reading challenge 2025">
  {{ page.pageread2 | times: 100 | divided_by: page.sayfa2 }}%
  </div>

  <div>
    <progress title="{{ page.pageread2 }}/{{ page.sayfa2 }}" value="{{ page.pageread2 }}" max="{{ page.sayfa2 }}" style="width: 80%;"></progress>
      <span style="font-size: 50%; font-style: italic;" title="reading challenge 2025">
      {{ page.pageread2 }}/{{ page.sayfa2 }}
      </span>
  </div>

  <br />
  <div style="clear: both"></div>

⁜ {{ page.read | plus: 3 }}

{{ page.booktitle3 }} ({{ page.bookyear3 }})  
_by_ {{ page.author3 }}

<div style="font-size: 50%; font-style: italic;"> {{ page.format3 }} </div>

  <div style="font-size: 50%; font-style: italic;">
  {{ page.sayfa3 }} sayfa
  </div>

  <div style="font-size: 50%; font-style: italic;" title="reading challenge 2025">
  {{ page.pageread3 | times: 100 | divided_by: page.sayfa3 }}%
  </div>

  <div>
    <progress title="{{ page.pageread3 }}/{{ page.sayfa3 }}" value="{{ page.pageread3 }}" max="{{ page.sayfa3 }}" style="width: 80%;"></progress>
      <span style="font-size: 50%; font-style: italic;" title="reading challenge 2025">
      {{ page.pageread3 }}/{{ page.sayfa3 }}
      </span>
  </div>

  <br />
  <div style="clear: both"></div>

⁜ {{ page.read | plus: 4 }}

{{ page.booktitle4 }} ({{ page.bookyear4 }})  
_by_ {{ page.author4 }}

<div style="font-size: 50%; font-style: italic;"> {{ page.format4 }} </div>

  <div style="font-size: 50%; font-style: italic;">
  {{ page.suresaat4 }} saat {{ page.suredakika4 }} dakika
  </div>

  <div style="font-size: 50%; font-style: italic;" title="reading challenge 2025">
  {{ page.pageread4 | times: 100 | divided_by: page.sayfa4 }}%
  </div>

  <div>
    <progress title="{{ page.pageread4 }}/{{ page.sayfa4 }}" value="{{ page.pageread4 }}" max="{{ page.sayfa4 }}" style="width: 80%;"></progress>
      <span style="font-size: 50%; font-style: italic;" title="reading challenge 2025">
      {{ page.pagereadsaat4 }}"{{ page.pagereaddakika4 }}'/{{ page.suresaat4 }}"{{ page.suredakika4 }}'
      </span>
  </div>

  <br />
  <div style="clear: both"></div>

  <br />
_Through the Year_

{% include image-gallery.html folder="/assets/through-the-year" %}

  <div style="clear: both"></div>
[🍃](https://www.next52books.com/now.html "şimdi okuduğum kitaplar")
