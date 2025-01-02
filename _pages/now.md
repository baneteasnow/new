---
# {{ 200 | times: 5 | divided_by: 100 }}
# {% include postcountbymonth.html %}
# Here's a sentence with a footnote. [^aaa]
# [^aaa]: This is the footnote.
# term
# : definition
#
read: 0
#
layout: page
title: şimdi okuduğum kitaplar
last_modified_at: 2025-01-01
published: true
#
# 1
booktitle1: "Stuff Every Coffee Lover Should Know"
bookyear1: 2024
author1: "Candace Rose Rardon"
sayfa1: 184
pageread1: 34
#
# 2
booktitle2: "Doppelganger"
bookyear2: 2024
author2: "Naomi Klein"
sayfa2: 416
pageread2: 1
#
# 3
booktitle3: "Empire of Pain"
bookyear3: 2024
author3: "Patrick Radden Keefe"
sayfa3: 632
pageread3: 30
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
# <div style="font-size: 50%; font-style: italic;" title="reading challenge 2024">
#   {{ page.pageread2 | times: 100 | divided_by: page.sayfa2 }}%
# </div>
#
# <div>
#   <progress title="{{ page.pageread2 }}/{{ page.sayfa2 }}" value="{{ page.pageread2 }}" max="{{ page.sayfa2 }}" style="width: 80%;"></progress>
#   <span style="font-size: 50%; font-style: italic;" title="reading challenge 2024">
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

  <div style="font-size: 50%; font-style: italic;">
   {{ page.sayfa1 }} sayfa
 </div>

 <div style="font-size: 50%; font-style: italic;" title="reading challenge 2024"> 
   {{ page.pageread1 | times: 100 | divided_by: page.sayfa1 }}%
 </div>

 <div>
   <progress title="{{ page.pageread1 }}/{{ page.sayfa1 }}" value="{{ page.pageread1 }}" max="{{ page.sayfa1 }}" style="width: 80%;"></progress>
   <span style="font-size: 50%; font-style: italic;" title="reading challenge 2024"> 
     {{ page.pageread1 }}/{{ page.sayfa1 }}
   </span>
 </div>

<br />
<div style="clear: both"></div>

⁜ {{ page.read | plus: 2 }}

{{ page.booktitle2 }} ({{ page.bookyear2 }})  
_by_ {{ page.author2 }}

  <div style="font-size: 50%; font-style: italic;">
  {{ page.sayfa2 }} sayfa
  </div>

  <div style="font-size: 50%; font-style: italic;" title="reading challenge 2024">
  {{ page.pageread2 | times: 100 | divided_by: page.sayfa2 }}%
  </div>

  <div>
    <progress title="{{ page.pageread2 }}/{{ page.sayfa2 }}" value="{{ page.pageread2 }}" max="{{ page.sayfa2 }}" style="width: 80%;"></progress>
      <span style="font-size: 50%; font-style: italic;" title="reading challenge 2024">
      {{ page.pageread2 }}/{{ page.sayfa2 }}
      </span>
  </div>

  <br />
  <div style="clear: both"></div>

⁜ {{ page.read | plus: 3 }}

{{ page.booktitle3 }} ({{ page.bookyear3 }})  
_by_ {{ page.author3 }}

  <div style="font-size: 50%; font-style: italic;">
  {{ page.sayfa3 }} sayfa
  </div>

  <div style="font-size: 50%; font-style: italic;" title="reading challenge 2024">
  {{ page.pageread3 | times: 100 | divided_by: page.sayfa3 }}%
  </div>

  <div>
    <progress title="{{ page.pageread3 }}/{{ page.sayfa3 }}" value="{{ page.pageread3 }}" max="{{ page.sayfa3 }}" style="width: 80%;"></progress>
      <span style="font-size: 50%; font-style: italic;" title="reading challenge 2024">
      {{ page.pageread3 }}/{{ page.sayfa3 }}
      </span>
  </div>

  <br />
  <div style="clear: both"></div>

  <br />
_Through the Year_

{% include image-gallery.html folder="/assets/through-the-year" %}

  <div style="clear: both"></div>
[🍃](https://www.next52books.com/now.html "şimdi okuduğum kitaplar")
