---
title: "Towards Extreme Generalization"
header:
    image: "assets/images/extremegen.jpg" 
    caption: "Photo credit: [**Viktor Forgacs**](https://unsplash.com/@sonance)"
show_date: True
date: "3rd April 2021"
classes: wide
author_profile: False
---
In his 2019 paper {% cite fchol%}, François Chollet provided one of the most comprehensive definitions of intelligence. He described intelligence as that which enables wild generalization across tasks, optimized specifically for flexibility and adaptability. 

Unfortunately trends in ML research today are a far cry from his description, leveraging unlimited priors to showcase superior performance at specific tasks, depicting the intelligence of the person involved in creating it rather than that of the algorithm. All of the SOTA in ML research today showcases the crystallized output of intelligence but not the process of intelligence itself.  

This brings us to the question of what the way forward is? Are neural networks the key to superior generalization or do we need a new framework altogether?

In my opinion, neural networks, atleast in the framework of: Training, Back-Prop, and Optimization are quite useless to achieve the state of superior generalization.

An agent which serves to generalize across multiple tasks needs to have a sense of uncertainty about it's priors. It must have the ability to decrease/increase that uncertainty on it's own, by a process which is independent of data. In order to escape from the bubble that unlimited training data provides, an agent needs to cut off it's reliance with data. Biological organisms seeem to do fine in this regard, so why can't ML agents?

The brain is a master of dealing with uncertainty. If we draw a superficial comparison with neural networks and the brain, you can see that they're both connected roughly the same. The complexity of their connections obscure both their dynamics (not for the lack of trying though {% cite dyn1 %},{% cite dyn2 %},{% cite dyn3 %},{% cite dyn4 %},{% cite dyn5 %} ), so we don't know how an input gets transformed as it passes through several layers. There are signifcant differences though. The brain doesn't work on back propagation {% cite bp1 %}, {% cite bp2 %} and has a control over it's experiences. It can assign relevance/determine validity because everything is uncertain, it is too fluid of an entity. Neural networks share the property of intractable dynamics with the brain but, they are forced to behave in a pre-determined way by the means of labels. Hard-coded labels enforce unknown constraints on the network, forcing it to either learn shortcut tricks (textures, patterns, colors etc.). If a network is trained solely to detect pictures of faces, it's behavior is morphed so as to "see" faces, whether it be in patterns, shortcut hacks or some other feature. So when it makes a mistake, it technically isn't a mistake from the perspective of the neural network, but a mismatch in perspective between what is true and what isn't. And this has to do with assigning labels. We need to rethink the way a neural network leans. A more flexible way. One which adapts constantly based on new data or ingrained priors(designed before training). Pre-defined datasets and hard-coded labels are the death of generalization.

### References
-------

{% bibliography --cited_in_order %}



