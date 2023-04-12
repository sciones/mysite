---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: splash
author_profile: false

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/library.jpg
  actions:
    - label: "Read Posts"
      url: "/posts/"
excerpt: "Read more and learn more, for knowledge is the key that unlocks the doors of opportunity, illuminates the path to success, and empowers you to navigate life's challenges."
intro: 
  - excerpt: "In today's world, finance, electronics engineering, and computer science are three of the most important and rapidly-evolving fields. Each of these disciplines plays a critical role in shaping the way we live, work, and interact with one another. From developing cutting-edge technologies to managing complex financial systems, professionals in these fields are at the forefront of innovation and progress. In this blog, we will explore the intersection of finance, electronics engineering, and computer science, and examine how these fields can work together to create new opportunities and drive positive change."
feature_row:
  - image_path: /assets/images/finance.jpg
    title: "Finance"
    excerpt: "The knowledge to take control of your money and making informed choices."
    url: "/categories/#finance"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/electronics.jpg
    title: "Electronics"
    excerpt: "Innovation powering the world and building the future."
    url: "/categories/#electronics"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/coding.jpg
    title: "Coding"
    excerpt: "Solving complex algorithms, one line of code at a time."
    url: "/categories/#coding"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

{% include id="intro"%}

{% include feature_row %}