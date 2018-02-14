<p align="center">
  <img height="150" src="https://github.com/tmscarla/TokenGame/blob/master/Logo/tokengame-original.png">
</p>
 
 
# TokenGame
This repo contains my Bachelor's thesis in Computer Engegneering at the University of Florence. Unfortunatly, the code that I developed will not be released open source, indeed here will be presented only the strategies, the methodologies and the patterns that I used. 

The written thesis (in italian), the slides of the presentation and some demo videos are present in the repo.

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


# Documentation

# Design

# API

# GUI


