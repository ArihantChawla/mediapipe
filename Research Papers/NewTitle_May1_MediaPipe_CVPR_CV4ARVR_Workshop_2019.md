MediaPipe: A Framework for Perceiving and Processing Reality
by Lugaresi, et al.

### Abstract 

* An app with Perceptual i/p involoves more than running not an ML model
* Balancing: 
	- devices,
	- resource usage,
	- quality of results,
	- run mutiple ops in  ||,
	- use piplelining to ensure time series data is properly synchronized

* What MEDIAPIPE does:
	- rapidly combines existing and new perception components and prototypes
	- advances them to polished cross platfoem apps
	- Resource Management can be configured using it (both CPU and GPU)
	- Dev can focus on Algo/Model and use MediaPipe as an env for iteratively improving apps and results are reproduciblr cross platform

*** 

### 1. Introduction 
* To enable AR, 
	- A typical app proc. sensory data such as A/V at high fps bc UX.
	- Plus there is strong coupleing between the steps
	- Developing the same app cross platform is a headache

* What MediaPipe Does: 
	- Abstracts and connects induvidual model into maintainable pipelines
	- Builds a perception pipleline as a graph of modular components (inference model, media proc functions, etc)

* About these Graphs of Modular Components:
	- I/P: Sensory Data (audio, vedio stream, etc)
	- O/P: [Egs] Object Detection results, Face Landmark annotations 

NOTE: Remember that Graphs of Ops. are used in projects like [tf](https://www.tensorflow.org/guide/intro_to_graphs), pytorch, cntk, etc.

	- MP. graphs are not about the internals of a NN
	- They specify large scale pipelines in which one or more models are implemented

