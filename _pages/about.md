---
permalink: /
# title: "Welcome to my website!"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
header:
  teaser: "unsplash-gallery-image-2-th.jpg"
---

# ![](/images/giesel.jpg)

About Me
======

I am a third year PhD student in [Mechanical and Aerospace Engineering](https://mae.ucsd.edu/) at UC San Diego, working with [Prof. Boris Kramer](http://kramer.ucsd.edu/index.html). My current research focuses on data-driven reduced-order modeling for applications to char combustion and semiconductor. 



News
======
**February 2025:** I am excited to be presenting our paper titled ["Computing Solutions to the Polynomial-Polynomial Regulator Problem"](https://arxiv.org/abs/2410.22291) at [CDC Milan 2024](https://cdc2024.ieeecss.org/). I am very proud of this work, which has produced my flagship [PPR GitHub repository](https://github.com/hyeonghun1/PPR) ; there you can find the main contribution from my CDC paper, the <span style="font-variant:small-caps;">Matlab</span> function `ppr()`, which functions analogously to the `lqr()` function but for nonlinear systems. Also provided is thorough documentation and some examples to get you started. My goal with this function is to make it fast and easy to compute nonlinear controllers with just one line of code, similar to <span style="font-variant:small-caps;"></span>'s built-in three-letter function `lqr()`. These controllers are essentially Taylor approximations to the true optimal control, so I always remind the properties of Taylor approximations: you can expect convergence to the true optimal control locally, i.e. better and better performance with higher degree feedback laws, but outside of the (unspecified) region of convergence of the Taylor expansion, these polynomial controllers will typically blow up and likely exhibit poor performance. I typically recommend starting with a degree 4 approximation to the value function, corresponding to a degree 3 optimal control approximation (the classic linear feedback is an odd function, so the next degree odd function is degree 3). In addition to better optimality locally, in some cases these controllers stabilize initial conditions that fail to be stabilized by LQR, although this is not guaranteed.