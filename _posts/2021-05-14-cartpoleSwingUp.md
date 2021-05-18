---
layout: single
title:  "Solving the cart-pole swing-up problem with energy shaping and LQR for stabilization"
date:   2021-05-14
---

In [Stabilizing the cart-pole system using finite-horizon LQR](https://blakerbuchanan.github.io/cartpoleLQR/), I discussed how one can implement an LQR controller to stabilize the cart-pole system when the system is initialized within the basin of attraction of the controlled system. This is satisfying in implementation, but one naturally then asks the question of how to accomplish the control problem of swinging up the pendulum when it is initialized outside of the basin of attraction. This was a neat result when I first successfully implemented it, and upon doing so a second time (in Julia), I still think it is neat.

The phrase "energy-shaping" is intuitive, answering the question: "how can I control the system such that it possesses a certain desired amount of energy?" I again assume the parameters are all equal to 1. Below is a video of my implementation of energy-shaping control. Continue reading for details concerning the method and implementation.
<div class="myvideo">
   <video  style="display:block; margin: 0 auto; width:70%; height:auto;" controls>
      <source src="{{ site.baseurl }}/viewable/cartpoleSwingUpv2.mp4" type="video/mp4" />
      <source src="{{ site.baseurl }}/viewable/cartpoleSwingUpv2.ogv" type="video/ogg" />
      <source src="{{ site.baseurl }}/viewable/cartpoleSwingUpv2.webm"  type="video/webm"  />
   </video>
</div>
<p>$$\text{A video of the final cart-pole swing-up control problem.}$$</p>

Details in progress. Topics will include feedback linearization and partial feedback linearization (collocated and noncollocated). Also show that this can be done with the Acrobot.
