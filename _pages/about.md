---
permalink: /
title: "About Me"
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
  - /home/
twitter-color: "#55acee"
github-color: "#171516"
blogger-color: "#F37100"
---

I am an **Associate Professor of Computer Science** at [Shenyang Aerospace University](https://www.sau.edu.cn/). Prior to this role, I completed my postdoctoral research under the guidance of Prof. [Shaogang Gong](https://www.eecs.qmul.ac.uk/~sgg/) at [Queen Mary University of London](https://www.qmul.ac.uk) in 2007. I earned my Ph.D. in Computer Science from [the University of York, UK](https://www.cs.york.ac.uk/) in 2006, where I was supervised by Prof. [Edwin Hancock (In Memoriam)](https://scholar.google.com/citations?user=EjDU2ncAAAAJ&hl=en). Additionally, I obtained my B.S. in Computer Science from [East China University of Science and Technology](http://www.ecust.edu.cn/) in 2001.  

I am the **founder** and **CEO** of [Shenyang Tymo Technology Co., Ltd.](https://www.tymo.cn) (abbreviated as Tymo Tech). Established in 2007, Tymo Tech is dedicated to applying computer vision and pattern recognition technologies in embedded products.  

<!-- This is a comment: Over the past decade, we have developed several products, including a crowd flow statistical system, a video perimeter system, image-based fire detectors, and light-section smoke detectors, which are widely used in firefighting, public safety, and transportation. -->  

I am also a **senior technical advisor** and **R&D director** at [Shenyang P.T. Security Technology Co., Ltd.](http://www.ptstec.cn) (abbreviated as PTS). PTS aims to become a professional manufacturer in the global industrial firefighting sector, and its research and production of temperature-sensing cable products are sold in over 30 countries.  

**Research Interests:** Reinforcement Learning, Graph Theory, Computer Vision  


 ---
<section id="News">  
    <h2>News</h2>  
    <div class="blog-posts">  
        {% assign recent_posts = site.posts | limit: 5 %}  <!-- Get the last 5 posts -->  
        {% for post in recent_posts %}  
            <article>  
                <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>  
                <p>{{ post.excerpt }}</p>  <!-- Display the post excerpt -->  
            </article>  
        {% endfor %}  
    </div>  
</section>