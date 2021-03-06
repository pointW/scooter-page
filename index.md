---
youtubeId: lDi9uFcD7XI
published: true
---

Assistive robot manipulators must be able to autonomously pick and place a wide range of novel objects to be truly useful. However, current assistive robots lack this capability. Additionally, assistive systems need to have an interface that is easy to learn, to use, and to understand. This paper takes a step forward in this direction. We present a robot system comprised of a robotic arm and a mobility scooter that provides both pick-and-drop and pick-and-place functionality for open world environments without modeling the objects or environment. The system uses a laser pointer to directly select an object in the world, with feedback to the user via projecting an interface into the world. Our evaluation over several experimental scenarios shows a significant improvement in both runtime and grasp success rate relative to a baseline from the literature ([Gualtieri _et al._](https://arxiv.org/abs/1609.05253)), and furthermore demonstrates accurate pick and place capabilities for tabletop scenarios.

<div style="text-align:center">
	<img src="img/system.png" alt="system" height="300"/>
  	<img src="img/interface.jpeg" alt="system" height="300"/>
</div>

The system is comprised of a Universal Robotics UR5 robot arm mounted on a Merits Pioneer 10 mobility scooter. Five StructIO depth sensors provide perception functionality for the system. The user interface, including a monitor, a key stick, a projector, and a dual laser pointer device, enable the system to interact with the user.

## Paper
Latest Version 3 Jun 2019: [arXiv:1809.09541[cs.RO]](https://arxiv.org/abs/1809.09541)

[Dian Wang<sup>1</sup>](https://pointw.github.io), 
[Colin Kohler<sup>1</sup>](https://www.ccis.northeastern.edu/people/colin-kohler/), 
Alexander Wilkinson<sup>2</sup>,
[Andreas ten Pas<sup>1</sup>](http://www.ccs.neu.edu/home/atp/), 
[Maozhi Liu<sup>1</sup>](https://www.linkedin.com/in/maozhi-liu/), 
[Holly Yanco<sup>2</sup>](http://www.cs.uml.edu/~holly/), 
[Robert Platt<sup>1</sup>](http://www.ccs.neu.edu/home/rplatt/)


<sup>1</sup>Northeastern University

<sup>2</sup>University of Massachusetts Lowell

```
@article{wang2019towards,
  title={Towards Assistive Robotic Pick and Place in Open World Environments},
  author={Wang, Dian and Kohler, Colin and Pas, Andreas ten and Wilkinson, Alexander and Liu, Maozhi and Yanco, Holly and Platt, Robert},
  journal={arXiv preprint arXiv:1809.09541},
  year={2019}
}
```


## Video
<div style="text-align:center">
	<iframe width="853" height="480" src="https://www.youtube.com/embed/ZimZlsJTaTU" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

## Experiments
### Grasping in Isolation

<div>
  <div style="float:left; width:450px;">
    <iframe width="400" height="225" src="https://www.youtube.com/embed/4sy7esFrItU?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
  </div>
  <div style="float:left; max-width:500px">
    <p>To evaluate the grasping functionality of our system, we performed experiments in a tabletop scenario where the scooter was stationary. For each trial, objects were placed on the table in randomly selected positions at least two centimeters away from each other in their upright orientation. These trials were run with automatic grasp selection in pick-and-drop mode by an expert user who determined the order the objects were grasped in.</p >
  </div>
</div>

<div style="clear:both"></div>
------
### Pick and Drop In-Situ
<div>
  <div style="float:left; width:450px;">
    <iframe width="400" height="225" src="https://www.youtube.com/embed/cfigrh8n-4s" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
  </div>
  <div style="float:left; max-width:500px">
    <p>To test our system in a real-world scenario, we used an open kitchen area. The system was run with automatic grasp selection in pick-and-drop mode by an expert user. At the start of each task, the scooter was driven to a start point and then up to the next object in the sequence to be grasped. Then the expert user would operate the system to grasp the target object.</p >
  </div>
</div>

<div style="clear:both"></div>
------
### Pick and Place In-Situ
<div>
  <div style="float:left; width:450px;">
    <iframe width="400" height="225" src="https://www.youtube.com/embed/T-kR89dqwQY" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
  </div>
  <div style="float:left; max-width:500px">
    <p>We tested the pick-and-place functionality in a more complex version of the kitchen environment. In each trial, objects were randomly assigned a target placing surface. These trials were run with manual grasp selection in pick-and-place mode by an expert user. At the start of each task, the scooter was driven to a start point and then up to the next object to be grasped. After the object was grasped, the scooter was driven to the target surface and the object was placed on top of it. </p >
  </div>
</div>

<div style="clear:both"></div>
------
### Comparing Maunal Grasp Selection with Automatic Grasp Selection
<div>
  <div style="float:left; width:450px;">
    <iframe width="400" height="225" src="https://www.youtube.com/embed/VT1dWXVGBXA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
  </div>
  <div style="float:left; max-width:500px">
    <p>To compare our manual grasp selection versus automatic grasp selection, we tested our system in dense objects setup. In each pair of trials, we ran the system to grasp target objects in the same sequence under automatic grasp selection and manual grasp selection in a similar pile, which is formed by placing objects on top of number tags.  </p >
  </div>
</div>

<div style="clear:both"></div>
------
### Failure Mode
#### Planning/IK Failure
<div>
  <div style="float:left; width:450px;">
    <iframe width="400" height="225" src="https://www.youtube.com/embed/XosmwToVDf0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
  </div>
  <div style="float:left; max-width:500px">
    <p>Because the distance between the arm and the sensor mounting bars was small, the arm's workspace was reduced and the system always suffers from no IK solution or planning failure. The video shows one particular grasping attempt, where the user had to reposition the platform multiple times to grasp the target object. The lack of RGB information in the interface also harmed the user's judgement. </p >
  </div>
</div>

<div style="clear:both"></div>

#### Pushing When Placing
<div>
  <div style="float:left; width:450px;">
    <iframe width="400" height="225" src="https://www.youtube.com/embed/8_BBPmg3g1c" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
  </div>
  <div style="float:left; max-width:500px">
    <p>Although we didn't take pushing as a failure in placing, it happened sometimes. </p >
  </div>
</div>

<div style="clear:both"></div>

<!-- ## System Workflow
### Interface WorkFlow
<div style="text-align:center">
	<img src="img/interface.png" alt="interface_flow" width="900"/>
</div>
### Grasping WorkFlow
<div style="text-align:center">
	<img src="img/grasping.png" alt="grasping_flow" width="700"/>
</div>
-->

## Contact
If you have any questions, please feel free to contact [Dian Wang](https://pointw.github.io) at wang[dot]dian[at]husky[dot]neu[dot]edu.
