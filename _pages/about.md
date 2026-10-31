---
layout: about
title: about
permalink: /
subtitle: 

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

I am a second-year Ph.D. student at Zhejiang University.

My research primarily focuses on diffusion models and generative modeling. My earlier work explored diffusion-based inverse problem solving, particularly in wireless channel estimation. 

I then shifted my focus to masked diffusion language models, with an emphasis on efficient inference and parallel decoding strategies. Currently, I am exploring **continuous diffusion language models**, particularly efficient text generation through **latent space compression**.


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

