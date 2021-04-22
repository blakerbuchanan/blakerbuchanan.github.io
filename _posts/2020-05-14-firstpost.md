---
layout: single
title:  "Stabilizing the cart-pole system using finite-horizon LQR"
date:   2021-04-21
---

<p>There are a variety of good resources for learning LQR and various other topics in optimal control. For this post, I have referenced Russ Tedrake's MIT online book [Underactuated Robotics](http://underactuated.mit.edu/index.html). In this post I will discuss the derivation of the LQR controller and its application to stabilizing the cart-pole system within some ball of its basin of attraction.</p>

<p>A fundamental feedback control strategy in optimal control is the linear quadratic regulator (LQR). It assumes linear dynamics of the form $$\dot{x} = Ax + Bu,$$ as well as a quadratic cost function given by $$J(x,u) = h(x(T)) + \int_0^T (x^TQx + u^TRu)dt.$$ It is also assumed that posti</p>
