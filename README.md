<p align="center">
  <img height="150" src="https://github.com/tmscarla/TokenGame/blob/master/Logo/tokengame-original.png">
</p>
 
 
# TokenGame
This repository contains my Bachelor's thesis in Computer Engegneering at the University of Florence. Unfortunately, the code that I developed will not be released open source, indeed here will be presented only the strategies, the methodologies and the patterns that I used. 

The written thesis (in italian), the slides of the presentation and some demo videos are anyway in the repository.

# Overview
The aim of the thesis was to design and develop a "token game" for Petri nets inside Oris, a tool developed from the [Software Technologies Lab](https://stlab.dinfo.unifi.it) of the [University of Florence](https://www.unifi.it) following consolidated methodologies theorized by the discipline of Software Engineering.

Basically, it is an interactive graphic interface that shows the evolution of the marking of a Petri net, giving the chance to evaluate some properties (such as the reachability) in a faster way. 

## Oris
[Oris](http://www.oris-tool.org) is a tool for qualitative verification and quantitative evaluation of reactive timed systems, which supports modeling and analysis of various classes of timed extensions of Petri Nets. As most characterizing features, Oris implements symbolic state space analysis of preemptive Time Petri Nets, which enable schedulability analysis of real-time systems running under priority preemptive scheduling.

Oris is a Java Maven project divided into several modules, each one with its specific function. Here we can see an UML component diagram: Sirio is the analysis engine which exposes APIs used by Oris. The Token Game API uses both Sirio and PetriNetLib, which is in turn used by the UI of the Token Game present in Oris.

<p align="center"><img height=300 src="https://github.com/tmscarla/TokenGame/blob/master/UML/OrisComponentDiagram.png"></p>

## Petri Net
A Petri net is a mathematical modeling languages for the description of distributed systems. It is a class of discrete event dynamic system. A Petri net is a directed bipartite graph, in which the nodes represent transitions (i.e. events that may occur, represented by bars) and places (i.e. conditions, represented by circles).

Petri nets offer a graphical notation for stepwise processes that include choice, iteration, and concurrent execution and they have also an exact mathematical definition of their execution semantics.

<p align="center"><img height=300 src="https://github.com/tmscarla/TokenGame/blob/master/Mockups/petrinetExample.png"></p>

# Analysis and Design

The requirements analysis phase has been driven through the use of use cases scenarios and diagrams. The main aim was to show the possible interactions of the user with the system, assuming an "user goal" layer of abstraction.

<p align="center"><img height=300 src="https://github.com/tmscarla/TokenGame/blob/master/UML/APIUseCaseDiagram.png"></p>

The following four use cases have been outlined:

* **Manual exploration:** the user can choose a particular transition to fire from a list of the available ones.
* **Automatic exploration:** make a random evolution of the net, according to two parameters:
  * *Steps*: maximum number of transitions that can fire in sequence
  * *Stop* condition: stop the exploration when a particular mark of the net is reached
* **Backtracking:** go back in the exploration for a finite number of steps.
* **Pick a history step:** the user can pick directly a previous state of the net to show detailed information

## Mockups
For the GUI, I developed some mockups using an application for prototyping: Balsamiq Mockups. 

<p align="center"><img height=300 src="https://github.com/tmscarla/TokenGame/blob/master/Mockups/TokenGame4.pdf"></p>

The window was divided into three different logical units:

* **Exploration:** enables the user to visualize the current state of the net and gathers all the possibile operations on it. Is itself divided into:
  * Selected state
  * Backtracking
  * Automatic exploration
* **Path history:** represents the path of the exploration, meaning all the states in which the net has gone trough. 
* **Petri net:** a visual representation of the Petri net.

# Development

## API

## GUI

## Implementation details

