---
permalink: /
excerpt: "Jiahe Dong's Personal Website"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am Jiahe Dong, currently pursuing my Master's degree in Computer Science at [ShanghaiTech University](https://www.shanghaitech.edu.cn/) [School of Information Science and Technology](https://sist.shanghaitech.edu.cn/) under the supervision of Prof. [Quan Li](https://faculty.sist.shanghaitech.edu.cn/liquan/) in the Viseer Lab.

My research interests primarily focus on **Data Visualization**, **Human Computer Interaction (HCI)**, **Interactions in Virtual Reality (VR) and Mixed Reality (MR)**, **Entertainment and Gamification**. I aim to make emerging technologies serve entertainment through human-computer interaction research.

## Education

**2025.6 - Present**  
**Master of Science in Computer Science**  
ShanghaiTech University, Shanghai, China  


**2021.9 - 2025.6**  
**Bachelor of Science in Computer Science**  
ShanghaiTech University, Shanghai, China

## Publications


{% assign publications = site.publications | reverse %}
{% for post in publications limit:3 %}
  {% include archive-single.html %}
{% endfor %}

[View all publications →]({{ '/publications/' | relative_url }})
