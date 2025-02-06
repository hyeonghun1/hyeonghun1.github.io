---
permalink: /
title: "Welcome to my website!"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
header:
  teaser: "unsplash-gallery-image-2-th.jpg"
---

![](/images/giesel.jpg)

About Me
======

I am a third year [Mechanical and Aerospace Engineering](https://mae.ucsd.edu/) PhD student at UC San Diego, working under [Prof. Boris Kramer](http://kramer.ucsd.edu/index.html). 
I have been working on efficient, scalable numerical methods for implementing nonlinear balanced truncation model reduction. 
Through that, my research broadened to the more general problem of scalable numerical methods for solving Hamilton-Jacobi-Bellman Partial Differential Equations, which naturally arise in nonlinear control theory. 
The success of linear control theory and linear model reduction stems directly from the availability of efficient, easy-to-use solvers; our goal is to develop these types of tools for nonlinear systems, since nonlinear, high-dimensional dynamical systems which are ubiquitous throughout science and engineering.
My current work on Kronecker product-based numerical methods for nonlinear balancing and nonlinear optimal control for high-dimensional systems can be found here on my GitHub!

My background is in Engineering Mechanics, which I studied during my BS and MS degrees at [Virginia Tech](https://beam.vt.edu/graduate/mechanics.html). 
During this time, I was exposed to a variety of problems, ranging from curiosity-driven science to aerospace-application driven problems, such as through my design teams and my internship at Pratt and Whitney. 
Furthermore, my master's work focused on vibration testing, specifically for railroad applications. 
Through all of these experiences, I was exposed to the need for general methods for efficiently simulating and analyzing complex engineering systems with features such as nonlinearity and complex geometry. 
This has motivated me to shift slightly towards the applied mathematics side of engineering to study model reduction methods during my PhD, which brought me to UCSD to work with Prof. Boris Kramer.


News
======
**December 2024:** I am also excited to be presenting our paper titled ["Computing Solutions to the Polynomial-Polynomial Regulator Problem"](https://arxiv.org/abs/2410.22291) at [CDC Milan 2024](https://cdc2024.ieeecss.org/). I am very proud of this work, which has produced my flagship [PPR GitHub repository](https://github.com/hyeonghun1/PPR) ; there you can find the main contribution from my CDC paper, the <span style="font-variant:small-caps;">Matlab</span> function `ppr()`, which functions analogously to the `lqr()` function but for nonlinear systems. Also provided is thorough documentation and some examples to get you started. My goal with this function is to make it fast and easy to compute nonlinear controllers with just one line of code, similar to <span style="font-variant:small-caps;"></span>'s built-in three-letter function `lqr()`. These controllers are essentially Taylor approximations to the true optimal control, so I always remind the properties of Taylor approximations: you can expect convergence to the true optimal control locally, i.e. better and better performance with higher degree feedback laws, but outside of the (unspecified) region of convergence of the Taylor expansion, these polynomial controllers will typically blow up and likely exhibit poor performance. I typically recommend starting with a degree 4 approximation to the value function, corresponding to a degree 3 optimal control approximation (the classic linear feedback is an odd function, so the next degree odd function is degree 3). In addition to better optimality locally, in some cases these controllers stabilize initial conditions that fail to be stabilized by LQR, although this is not guaranteed.

**December 2024:** I just finished visiting [Prof. Alessandro Alla](https://www.alessandroalla.com) at La Sapienza, University of Rome. I am very grateful for the opportunity to visit and discuss our common research interests of model reduction and control of dynamical systems. E per chi non lo sapesse, sono metá italiano, quindi é stata una grande opportunita visitare Roma e parlare con alcuni ricercatori italiani molto gentili. 

**November 2024:** Our paper titled "Scalable Computation of $\mathcal{H}_\infty$ Energy Functions for Polynomial Control-Affine Systems" was recently accepted to [IEEE Transactions on Automatic Control](https://doi.org/10.1109/TAC.2024.3494472). This paper presents the theory behind using Taylor approximations to compute the energy functions for control-affine dynamical systems with nonlinear drift, input, and output. The associated code can be found [here](https://github.com/hyeonghun1/NLbalancing) on my GitHub.

**September 2024:** We recently started work on a new multi-university research initiative (MURI) on the[ mathematics for digital twins](https://ai-dt.su.domains/). We are interested in using model reduction techniques for nonlinear control, with particular interest in laser powder bed fusion (PBF). This advanced 3D printing, also known as additive manufacturing, technique enables developing very complex part geometries, but many open problems exist regarding the optimization of control parameters such as the laser power, speed, and the path-planning corresponding to the slicing process. In particular, sub-optimal slicing and parameters can cause significant warping and even cracking of printed parts. We hope to advance the use of model reduction to tackle some of these challenges while advancing the broader approach of pairing real-world measurements with computer models, an idea known as digital twins. 

**September 2024:** We had a wonderful time hosting this year's [MORe2024](https://more2024.sciencesconf.org) here in beautiful La Jolla at the Scripps seaside conference venue. 
I presented the most recent state-of-the-art in computational methods for Nonlinear Balanced Truncation, based on our [IEEE Transactions paper on computing energy functions](https://doi.org/10.1109/TAC.2024.3494472) and [our recently submitted paper on computing balancing transformations](https://arxiv.org/abs/2410.22435). 
We always welcome visitors to San Diego and appreciate everyone who took the time to come and discuss/present their research.
