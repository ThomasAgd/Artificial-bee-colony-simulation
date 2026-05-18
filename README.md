# Artificial Bee Colony Simulation

Artificial Bee Colony (ABC) simulation inspired by the food-search behaviour of honey bees.

This project models the interactions between different bee roles and food sources inside a dynamic environment.

The simulation explores concepts such as:

- Multi-agent systems
- Swarm intelligence
- Graph exploration
- Behaviour simulation
- Object-oriented design
- Real-time visualisation

---

## Overview

The project reproduces the behaviour of an artificial bee colony composed of:

### Scouts

Responsible for exploring the environment and identifying food sources.

Responsibilities:

- Environment exploration
- Node discovery
- Source selection
- Communication with employees

### Employees

Workers assigned to discovered food sources.

Responsibilities:

- Source exploitation
- Neighbour evaluation
- Quality comparison
- Local optimisation

### Observers

Special agents analysing colony activity.

Responsibilities:

- Observation of selected nodes
- Probabilistic assignment
- Reinforcement of promising sources

---

## Architecture

```text
Bee
│
├── Scout
│
├── Employee
│
└── Observer
```

Additional entities:

- Node
- Terrain
- Sound
- TitleScreen
- EndScreen

The hierarchy is entirely based on object-oriented design principles.

---

## Environment Model

The simulation environment is composed of:

### Nodes

Each node represents a food source.

Attributes include:

- Identifier
- Coordinates
- Quality score
- Visit counters
- Visual colour mapping
- Best source tracking

Node colours change dynamically according to quality:

- Low quality: Blue tones
- High quality: Red tones

This allows visual identification of attractive resources.

---

## Graph Representation

Food sources are connected using a graph structure.

Implemented structures:

```java
HashMap<Integer, Node> nodes;

HashMap<Integer, ArrayList<Integer>> links;
```

The graph stores:

- Nodes
- Neighbour relations
- Reachability information
- Exploration paths

Connections are created according to spatial proximity.

---

## Data Structures

### ArrayLists

Used for:

- Scouts
- Employees
- Observers
- Available nodes
- Selected nodes
- Exploration queues

Examples:

```java
ArrayList<Scout> scouts;

ArrayList<Employee> employees;

ArrayList<Observer> observers;
```

### HashMaps

Used for:

- Fast node access
- Graph links
- Neighbour search

---

## Simulation Workflow

```text
Initialisation
      ↓
Environment generation
      ↓
Node creation
      ↓
Graph construction
      ↓
Scout exploration
      ↓
Employee assignment
      ↓
Neighbour optimisation
      ↓
Observer evaluation
      ↓
Visual update
      ↓
Repeat
```

---

## Behaviour System

### Exploration Phase

Scouts move across the terrain searching for promising nodes.

### Exploitation Phase

Employees exploit selected food sources.

They may:

- revisit nodes
- evaluate neighbours
- switch to better sources

### Observation Phase

Observers analyse colony decisions and reinforce efficient choices.

---

## Main Components

### Bee

Base entity controlling:

- Position
- Speed
- Animation
- Movement
- Target selection
- Return to hive

### Node

Represents food sources.

Contains:

- Coordinates
- Quality value
- State information
- Visit tracking

### Terrain

Main simulation manager.

Responsibilities:

- Environment generation
- Node placement
- Link creation
- Agent management
- Rendering
- Simulation loop

---

## Additional Features

Implemented interface elements:

✓ Title screen

✓ End screen

✓ Background music

✓ Dynamic colours

✓ Animated agents

✓ Real-time rendering

The project includes an original soundtrack composed specifically for the simulation.

---

## Technologies

Language:

- Java

Concepts:

- Object Oriented Programming
- Multi-agent simulation
- Swarm intelligence
- Graph theory
- Behaviour modelling
- Real-time systems

Data structures:

- ArrayList
- HashMap
- Graph representation

---

## Visual Features

The simulation displays:

- Bees movement
- Food nodes
- Graph links
- Resource quality
- Colony behaviour
- Environment updates

Visual information changes dynamically during execution.

---

## Educational Objectives

This project explores:

- Artificial Bee Colony algorithms
- Multi-agent interactions
- Behaviour simulation
- Resource optimisation
- Graph traversal
- Object-oriented architecture

---

## Possible Improvements

Future developments:

- Genetic optimisation
- Pathfinding algorithms
- Performance monitoring
- Statistics dashboard
- Colony metrics
- Heatmaps
- Resource evolution tracking
- Export system
- Replay mode

---

## Academic Context

Project developed during the second year of Computer Science degree.

Main themes:

- Java
- Object-oriented programming
- Simulation systems
- Agent modelling
- Graph structures
- Algorithmic optimisation

---

## Authors

Thomas Augendre  
Elyes Medjani
