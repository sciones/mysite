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
excerpt: "Read more, learn more, for knowledge is the key that unlocks the doors of opportunity, illuminates the path to success, and empowers you to navigate life's challenges."
intro: 
  - excerpt: "Welcome to our blog, where we explore the fascinating worlds of finance, electronics engineering, and computer science. Our engaging contents will inspire you to learn more about these exciting and dynamic fields."
feature_row:
  - image_path: /assets/images/finance.jpg
    title: "Finance"
    excerpt: "The knowledge to take control of your money and making informed choices."
    url: "/finance/"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/electronics.jpg
    title: "Electronics"
    excerpt: "Innovation powering the world, building the future."
    url: "/electronics/"
    btn_label: "Read More"
    btn_class: "btn--secondary"
  - image_path: /assets/images/coding.jpg
    title: "Coding"
    excerpt: "Solving complex algorithms, one line of code at a time."
    url: "/coding/"
    btn_label: "Read More"
    btn_class: "btn--success"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}