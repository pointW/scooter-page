---
youtubeId: lDi9uFcD7XI
published: true
---

Many people with motor disabilities struggle with activities of daily life (ADLs), limiting their ability to live independently. This paper details a robotic mobility scooter developed to assist with manipulation-based ADLs to increase independence. We present a system comprised of a Universal Robotics UR5 robotic arm, a mobility scooter, five depth sensors, and a user interface which utilizes laser pointers. The system provides pick-and-drop and pick-and-place functionality in open world environments without modeling the objects or environment. We evaluate our system over several experimental scenarios and show an improvement relative to a baseline established for a similar system.

<div style="text-align:center">
	<img src="img/system.JPG" alt="system" height="300"/>
  	<img src="img/interface.JPG" alt="system" height="300"/>
</div>

The system is comprised of a Universal Robotics UR5 robot arm mounted on a Merits Pioneer 10 mobility scooter. Five StructIO depth sensors provide perception functionality for the system. The user interface, including a monitor, a key stick, and a dual laser pointer device, enable the system to interact with the user.

## Paper
Latest Version 25 Sep 2018: [arXiv:1809.09541[cs.RO]](https://arxiv.org/abs/1809.09541)

Submmited to IEEE International Conference on Robotics and Automation (ICRA) 2019

[Dian Wang<sup>1</sup>](https://pointw.github.io), 
[Colin Kohler<sup>1</sup>](https://www.ccis.northeastern.edu/people/colin-kohler/), 
[Andreas ten Pas<sup>1</sup>](http://www.ccs.neu.edu/home/atp/), 
[Maozhi Liu<sup>1</sup>](https://www.linkedin.com/in/maozhi-liu/), 
[Holly Yanco<sup>2</sup>](http://www.cs.uml.edu/~holly/), 
[Robert Platt<sup>1</sup>](http://www.ccs.neu.edu/home/rplatt/)


<sup>1</sup>Northeastern University

<sup>2</sup>University of Massachusetts Lowell

## Video
<div style="text-align:center">
	<iframe width="853" height="480" src="https://www.youtube.com/embed/-FqXRtMlc4U" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

## Experiments
### Grasping in Isolation

<div>
  <div style="float:left; width:450px;">
    <iframe width="400" height="225" src="https://www.youtube.com/embed/4sy7esFrItU?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
  </div>
  <div style="float:left; max-width:500px">
    <p>To evaluate the grasping functionality of our system, we performed experiments in a tabletop scenario on a 46 cm tall table while the scooter was stationary. For each trial, six objects were randomly selected from the object set and placed on the table in randomly selected positions at least two centimeters away from each other in their upright orientation. These trials were run with automatic grasp selection in pick-and-drop mode by an expert user who determined the order the objects were grasped in.</p >
  </div>
</div>

<div style="clear:both"></div>

### Pick and Place In-Situ
<div>
  <div style="float:left; width:450px;">
    <iframe width="400" height="225" src="https://www.youtube.com/embed/cfigrh8n-4s" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
  </div>
  <div style="float:left; max-width:500px">
    <p>To test our system in a real-world scenario, we used an open kitchen area. The system were run with automatic grasp selection in pick-and-drop mode by an expert user. At the start of each task, the scooter was driven to a start point and then up to the next object in the sequence to be grasped. Then the expert user would operate the system to grasp the target object.</p >
  </div>
</div>

<div style="clear:both"></div>

## System Workflow
### Interface WorkFlow
<div style="text-align:center">
	<img src="img/interface.png" alt="interface_flow" width="700"/>
</div>
### Grasping WorkFlow
<div style="text-align:center">
	<img src="img/grasping.png" alt="grasping_flow" width="700"/>
</div>
