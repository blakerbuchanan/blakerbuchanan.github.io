---
title:  "Research"
layout: archive
permalink: /Research/
author_profile: true
comments: true
---

## Biography

I graduated cum laude from the University of North Carolina at Charlotte in 2018 where I earned a BS in Mechanical Engineering and Engineering Science. I worked on an array of different research and engineering projects, culminating in my passion for graduate studies and research. My research efforts took place throughout my final two years, during which I was advised by Professor <a href="http://scottdavidkelly.wikidot.com/">Scott D. Kelly</a>. I then went on to graduate with a MS in robotics in 2020 from Carnegie Mellon University's Robotics Institute. I was associated with the <a href="http://biorobotics.ri.cmu.edu/index.php">Biorobotics</a> lab and was co-advised by Professors <a href="https://www.ri.cmu.edu/ri-faculty/howie-choset/">Howie Choset</a> and <a href="https://www.ri.cmu.edu/ri-faculty/matthew-j-travers/">Matthew Travers</a>, with Professor Kelly also closely involved in my research development. I currently reside at the Robotics Institute as a researcher in the Biorobotics lab. My focus has primarily been on studying, developing models for, and building multi-agent systems of underactuated robots rooted in nonholonomic mechanics that embody biological agents whose locomotion are coupled through compliant substrates or fluids.

<!---## Mechanics and Control of Coupled Interactions in Ambient Media-->
<details>
  <summary>Mechanics and Control of Coupled Interactions in Ambient Media</summary>
<p>Mechanical systems exhibiting nonholonomic constraints can often be of utility in the study of locomotion and coupled group behaviors for biological systems. Many multi-agent systems in nature, for example, are comprised of agents that interact with, and respond to, the dynamics of their environment. In a recent paper, we approached the study of such agent-environment interactions through the study of passively compliant vehicles coupled to their environment via simple nonholonomic constraints. The Chaplygin beanie is a simple underactuated mechanical system that locomotes when its rotor rotates relative to its body. An example of the Chaplygin beanie is shown below. Supported by two frictionless casters at the front and a torsional spring coupling the rotor to the cart, a nonzero displacement in the spring induces locomotion.</p>
<br />
<div style="text-align: center"><img src="{{ site.baseurl }}/assets/imgs/beanieOnAPlatformPic.png" alt="Chaplygin beanie on a movable platform"></div>
<br />
<p>The Chaplygin beanie is shown sitting atop a passive platform capable of translational motion. In our recent paper published in the ASME 2020 Dynamic Systems and Control Conference <a href="https://blakerbuchanan.github.io/Publications/">(1)</a>, we prove that all initial conditions corresponding to zero net momentum of this mechanical system will result in stable forward motion of the Chaplygin beanie. In particular, when its rotor is wound up arbitrarily, the behavior in the following video is exhibited.</p>
<br />
<div class="myvideo">
   <video  style="display:block; width:70%; height:auto;" controls>
      <source src="{{ site.baseurl }}/viewable/beanieplatformcropped.mp4" type="video/mp4" />
      <source src="/viewable/beanieplatformcropped.ogv" type="video/ogg" />
      <source src="/viewable/beanieplatformcropped.webm"  type="video/webm"  />
   </video>
</div> 
<br />
<p>The paper referenced above also explores control of the platform, termed <em>exogenous control</em>, and the resulting locomotion of a passive Chaplygin beanie. Much of the work in this paper also contributed to my Master's thesis, which you can download <a href="https://www.ri.cmu.edu/publications/mechanics-and-control-of-coupled-interactions-in-ambient-media/">here</a>.</p>
</details>

<!---## Communication Through Ambient Media-->
<details>
  <summary>Communication Through Ambient Media</summary>
  
  <p>This coupling between agents through ambient media can also be viewed as a mechanism for communication. Communication through some physical media has been termed <em>mechanical communication</em> and has been shown to be exhibited at the cellular level (see <a href="https://www.nature.com/articles/nphys3619">this</a>). This particular form of communication is distinct in that information flows through a medium possessing dynamics of its own, encoding quantities possibly describing an individual agent's behavioral states, disturbances in the surrounding medium, and overall group behavioral states. My previous work began to lay a theoretical foundation for investigating mechanical communication from a perspective of robotics and applied mathematics. My current work involves further establishing the concept of mechanical communication within multi-agent systems in ambient media and determining how it can be exploited for decision-making and control of collections of agents within these systems. More on this work as it develops :) </p>
</details>

<details>
  <summary>Snake Robot Locomotion</summary>
  <p>The constraints on a snake as it slithers along the ground can also be modeled as nonholonomic constraints on a series of wheels on a series of articulated linkages. The role of compliance in biological systems is ubiquitous. Fish and snakes have flexible bodies, and humans have muscles and tendons which are compliant. In <a href="https://blakerbuchanan.github.io/Publications/">(2)</a>, we investigate the locomotion of a multi-link nonholonomic snake robot and experimentally validate its locomotion under amplitude and frequency variations in sinusoidal actuation of its foremost joint. The remaining joints are passively compliant via linear springs. A robot of such a system is shown below.</p>
    <div style="text-align: center"><img src="{{ site.baseurl }}/assets/imgs/side.jpg" alt="Snake robot with four links"></div>
  <p>And here is a video of that robot undergoing a prescribed amplitude modulation to locomote around an object in its environment.</p>
  <div class="myvideo">
    <video  style="display:block; width:70%; height:auto;" controls>
      <source src="{{ site.baseurl }}/viewable/fourlinkspeedobject.mp4" type="video/mp4" />
      <source src="/viewable/fourlinkspeedobject.ogv" type="video/ogg" />
      <source src="/viewable/fourlinkspeedobject.webm"  type="video/webm"  />
    </video>
  </div> 
  <p>Robots like this one help us to describe the locomotion of biological systems. I hope to develop more of these kinds of robots in some of my future work with multi-agent systems in ambient media to gain some fundamental insight into how such media contributes to the coordinated efforts of organisms like fish and even cells.
</details>

