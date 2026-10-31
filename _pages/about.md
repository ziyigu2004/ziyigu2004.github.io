---
layout: about
title: about
permalink: /
subtitle: Ph.D. Student at Zhejiang University

profile:
  align: right
  image: imag_me.jpg
  image_circular: false
  more_info: >
    <p>Zhejiang University</p>
    <p>Hangzhou, China</p>

selected_papers: false
social: false

announcements:
  enabled: false

latest_posts:
  enabled: false
---

<section id="about"></section>

## About Me

I am a Ph.D. student in Information and Communication
Engineering at Zhejiang University.

My research focuses on diffusion models and generative
modeling, particularly diffusion language models and
efficient inference methods.

## Research Interests

- Efficient Inference for Diffusion Language Models
- Continuous Diffusion Language Models
- Diffusion Models for Inverse Problems

<section id="publications"></section>

## Publications

<div class="publications">
{% bibliography --file papers %}
</div>

<section id="contact"></section>

## Contact

- Email: [heqiangqi@zju.edu.cn](mailto:heqiangqi@zju.edu.cn)
- GitHub: [ziyigu2004](https://github.com/ziyigu2004)


<script>
document.addEventListener("DOMContentLoaded", function () {
  const publications = document.querySelector(
    '.navbar-nav a[href="/publications/"]'
  );

  if (!publications) return;

  const contactItem = document.createElement("li");
  contactItem.className = "nav-item";

  const contactLink = document.createElement("a");
  contactLink.className = "nav-link";
  contactLink.href = "/#contact";
  contactLink.textContent = "Contact";

  contactItem.appendChild(contactLink);
  publications.parentElement.insertAdjacentElement(
    "afterend", contactItem
  );
});
</script>

