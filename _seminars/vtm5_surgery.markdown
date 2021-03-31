---
layout: page
title: Automation of Surgical Tasks Using Hybrid Dynamical Systems
description: VTM5 by Michele Ginesi
img: #/assets/img/vtm3-thumbnail.png
importance: -20210309 # date in format '-YYYYMMDD'
---


Recording: [Link](https://univr.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=ba8c3e62-89c2-4a68-9be7-ace6016591f8)

Automation of **Robotic Minimally Invasive Surgery** holds significant promise to improving patient treatment, reduce recovery time, and reduce the fatigue of the surgeons. To achieve automation in surgical robotics, multiple challenges must be addressed (e.g. scene recognition, planning, control, etc.). Surgeons master their skills with years of training, and gestures are performed using muscular memory and expertise. In this seminar, we will talk about gesture learning and segmentation. We will present a **Hybrid Dynamical System** (HDS), i.e., a system composed of both a discrete and a continuous component. The **discrete** component determines the currently active mode, and each mode describes the continuous evolution of the robot's end-effector position. For instance, the suturing task can be subdivided into many gestures (looping, knot-tying, etc.). Each gesture is a mode, and it can be achieved by performing a particular movement with the robot end-effector. Modeling the surgical task as an HDS allows learning both the continuous evolution and the mode transition rules from observations of real surgical tasks. The **continuous** component of the HDS is modeled using the Dynamic Movement Primitives (DMPs) framework, which allows learning trajectories of any shape. To learn the mode transition rules, a segmentation of the surgical task into segments is needed. Manual segmentation is a tedious process, and errors are practically unavoidable. Thus, we propose an unsupervised method based upon the **Auto-Regressive Hidden Markov Model**. The seminar will first introduce the problem of automation in Minimally Invasive Surgery. Then, we will present our proposed HDS model. Finally, some preliminary results in the automation of surgical-related tasks will be presented.

**Michele Ginesi** is a former student of the bachelor and master programmes in Mathematics of the University of Verona and is now a PhD student in Computer Science. His research interests cover the fields of hybrid dynamical systems and autonomous task planning.
