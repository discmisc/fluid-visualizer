# Fluid Simulation Project

## Overview

This project is a simple fluid simulation implemented using HTML5 Canvas and JavaScript. It provides a basic visualization of fluid dynamics, including velocity vectors and pressure.

## Features

- Fluid simulation using a grid-based approach
- Visualization of pressure, velocity, and smoke (density)
- Interactivity: Users can introduce obstacles to the fluid flow by clicking and dragging on the canvas.

## Getting Started

### Prerequisites

Make sure you have a modern web browser that supports HTML5 Canvas.

### Running the Simulation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/fluid-simulation.git
   cd fluid-simulation

2. Open the **index.html** file in your preferred web browser.

## Configuration

Adjust simulation parameters in the JavaScript code as needed:

1. **`numX`** and **`numY`**: Number of grid cells in the X and Y directions.
2. **`h`**: Grid spacing.
3. Other parameters related to fluid properties.

### Usage
1.Click and drag on the canvas to introduce obstacles to the **`fluid flow`**.

2.Observe the simulation of fluid dynamics, including `pressure`, `velocity`, and `smoke`.


### Explanation

The project visualises the grid-spacing, pressure, density and noise impact on the flow of a Eulerian Fluid.

## Eulerian Fluid

The Eulerian Description is one in which a control volume is defined, within which fluid flow properties of interest are expressed as fields. Grave to note, that it follows the Grid-Arrangement

![Link Name](https://github.com/discmisc/fluid-visualizer/blob/main/images/e_fluid.png)  

### Incompressibility of Eulerian Fluids

The incompressibility of Eulerian fluids is a key concept in fluid dynamics, particularly within the framework of the Euler equations describing inviscid fluid motion. In this context, the assumption of incompressibility simplifies the mathematical representation of the fluid's behavior. The Euler equations, derived from mass and momentum conservation, include a mass conservation equation. For incompressible fluids, this simplifies to the divergence-free condition (∇⋅u=0), indicating constant density. This assumption is applicable to liquids and gases at low speeds, allowing for efficient mathematical treatment and numerical simulations in fields such as aerodynamics and hydrodynamics. Incompressibility implies negligible density variations, making it a valuable approximation for understanding and predicting fluid dynamics phenomena while facilitating practical applications in engineering and computational fluid dynamics.

In fluid dynamics, ensuring incompressibility involves maintaining constant density throughout the flow. The mentioned phrase emphasizes that a fluid cannot arbitrarily alter one velocity component without considering the overall system. If an excessive inflow were to change a single velocity independently, it would violate the incompressibility condition.

To enforce incompressibility effectively, any adjustments in the fluid's velocity field must be coherent. The directive to "Push all velocities outward by the same amount" underscores the need for a simultaneous and uniform modification of velocities. This coherent adjustment ensures that density remains constant, aligning with the incompressibility assumption. In essence, it reflects the concerted effort required to preserve fluid incompressibility while making adjustments to its velocity field.

![Link Name](https://github.com/discmisc/fluid-visualizer/blob/main/images/imposing_compression.png)  

### Usage of Obstacles

In the context of enforcing incompressibility in fluid dynamics, obstacles play a crucial role in shaping and directing the flow. Introducing obstacles within a fluid domain serves as a practical means to control and guide the fluid while adhering to the incompressibility constraint.

Obstacles act as constraints on the fluid motion, influencing the velocity field in their vicinity. By strategically placing obstacles, engineers and researchers can manipulate the fluid dynamics to achieve specific objectives. For instance, obstacles can be employed to induce desired patterns of circulation, enhance mixing, or control the direction of flow.

In the quest for incompressible flow, obstacles aid in distributing and redirecting velocities uniformly. They help prevent localized variations that might compromise the overall incompressibility of the fluid. Whether in the design of channels, nozzles, or other fluidic devices, obstacles become integral components for achieving and maintaining incompressibility in practical applications.

![Link Name](https://github.com/discmisc/fluid-visualizer/blob/main/images/usage_obstacles.png)  

