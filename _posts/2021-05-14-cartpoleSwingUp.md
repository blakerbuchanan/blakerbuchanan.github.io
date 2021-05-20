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

Our goal is to inject energy into the system in a controlled way such that it possesses an amount of energy corresponding to the unstable fixed point. To do this, we first need to linearize part of the dynamics so that we are working only with a subset of the *nonlinear* dynamics. The linearization of part of the dynamics of a system is appropriately called *partial feedback linearization* (PFL). There are two distinct types of PFL: *collocated* and *non-collocated*. We employ collocated PFL if we want to linearize the dynamics of actuated variables, and employ non-collocated PFL when we want to linearize the dynamics of unactuated variables. Collocated PFL yields the following equations (the same as those obtained in [Underactuated Robotics](http://underactuated.mit.edu/index.html) when parameters are equal to 1):

$$ \ddot{\theta} = -\ddot{x}\cos\theta - \sin\theta,$$
$$ \ddot{x}(2-\cos^2\theta) - \sin\theta\cos\theta-\dot{\theta}^2\sin\theta = f_x.$$


