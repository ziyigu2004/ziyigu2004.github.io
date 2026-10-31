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
    <h2 style="font-size: 28px; font-weight: 700; margin-top: 18px; margin-bottom: 12px;">Heqiang Qi</h2>
    <p>Zhejiang University</p>
    <p>Hangzhou, China</p>

selected_papers: false
social: false

announcements:
  enabled: false

latest_posts:
  enabled: false
---


<style>
/* 隐藏顶部自动生成的姓名 */
.post-header .post-title {
    display: none;
}

/* 减少隐藏姓名后留下的空白 */
.post-header {
    margin-bottom: 0;
}

/* Publications 标题与上文之间增加间距 */
h2#publications {
    margin-top: 155px;
    margin-bottom: 32px;
}

/* Contact 与上方论文内容增加间距 */
h2#contact {
    margin-top: 45px;
}
</style>


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

