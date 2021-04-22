---
layout: single
title:  "Stabilizing the cart-pole system using finite-horizon LQR"
date:   2021-04-21
---

<p>A fundamental feedback control strategy in optimal control is the linear quadratic regulator (LQR). It assumes linear dynamics of the form $$\dot{x} = Ax + Bu,$$ as well as a quadratic cost function given by $$J(x,u) = h(x(T)) + \int_0^T (x^TQx + u^TRu)dt.$$</p>
