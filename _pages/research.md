---
title:  "Research"
layout: archive
permalink: /Research/
author_profile: true
comments: true
---

## Biography

I graduated cum laude from the University of North Carolina at Charlotte in 2018 where I earned a BS in Mechanical Engineering and Engineering Science. I worked on an array of different research and engineering projects, culminating in my passion for graduate studies and research. My research efforts took place throughout my final two years, during which I was advised by Professor <a href="http://scottdavidkelly.wikidot.com/">Scott D. Kelly</a>. I then went on to graduate with a Master's in robotics in 2020 from Carnegie Mellon University's Robotics Institute. I am associated with the <a href="http://biorobotics.ri.cmu.edu/index.php">Biorobotics</a> lab and was co-advised by Professors <a href="https://www.ri.cmu.edu/ri-faculty/howie-choset/">Howie Choset</a> and <a href="https://www.ri.cmu.edu/ri-faculty/matthew-j-travers/">Matthew Travers</a>, with Professor Kelly also closely involved in my research development. My focus has primarily been on studying, developing models for, and building multi-agent systems of underactuated robots rooted in nonholonomic mechanics that embody underlying principles of biological agents coupled through compliant substrates or fluids.

## Mechanics and Control of Coupled Interactions in Ambient Media
Mechanical systems exhibiting nonholonomic constraints can often be of utility in the study of locomotion and coupled group behaviors for biological systems. Many multi-agent systems in nature, for example, are comprised of agents that interact with, and respond to, the dynamics of their environment. In a recent paper, we approached the study of such agent-environment interactions through the study of passively compliant vehicles coupled to their environment via simple nonholonomic constraints. The Chaplygin beanie is a simple underactuated mechanical system that locomotes when its rotor rotates relative to its body. An example of the Chaplygin beanie is shown below. Supported by two frictionless casters at the front and a torsional spring coupling the rotor to the cart, a nonzero displacement in the spring induces locomotion.
<br />
<div style="text-align: center"><img src="{{ site.baseurl }}/assets/imgs/beanieOnAPlatformPic.png" alt="Chaplygin beanie on a movable platform"></div>
<br />
The Chaplygin beanie is shown sitting atop a passive platform capable of translational motion. In our recent paper published in the ASME 2020 Dynamic Systems and Control Conference (1), we prove that all initial conditions corresponding to zero net momentum of this mechanical system will result in stable forward motion of the Chaplygin beanie. In particular, when its rotor is wound up arbitrarily, the behavior in the following video is exhibited.
<br />
<div class="myvideo">
   <video  style="display:block; width:70%; height:auto;" controls>
      <source src="{{ site.baseurl }}/viewable/beanieplatformcropped.mp4" type="video/mp4" />
      <source src="/viewable/beanieplatformcropped.ogv" type="video/ogg" />
      <source src="/viewable/beanieplatformcropped.webm"  type="video/webm"  />
   </video>
</div> 
<br />
The paper referenced above also explores control of the platform, termed <em>exogenous control</em>, and the resulting locomotion of a passive Chaplygin beanie. Much of the work in this paper also contributed to my Master's thesis, which you can download <a href="https://www.ri.cmu.edu/publications/mechanics-and-control-of-coupled-interactions-in-ambient-media/">here</a>.
