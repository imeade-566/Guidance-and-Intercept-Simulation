# Guidance-and-Intercept-Simulation

A MATLAB-based aircraft engagement simulation developed to model and evaluate
autonomous interceptor guidance against a maneuvering target.

The simulation achieved approximately **91% intercept success across 32,980
randomized engagement scenarios** using proportional-navigation and lofted
guidance, line-of-sight loss handling, obstacle avoidance, and autonomous
target-evasion behavior.

## Project Overview

This project was developed to explore missile guidance, target tracking, and
autonomous decision-making in a configurable simulated engagement environment.

Rather than evaluating a single predetermined trajectory, the simulation can
run large batches of randomized engagements to evaluate guidance performance
across varying initial conditions and engagement geometries.

The project includes both individual live simulations for visualizing an
engagement and batch testing for evaluating overall system performance.

## Key Features

- Proportional Navigation (PN) guidance
- Lofted trajectory guidance
- Autonomous evasive target behavior
- Line-of-sight loss handling and target propagation
- G-limited maneuvering
- Artificial Potential Field (APF) obstacle avoidance
- Randomized engagement generation
- Batch/Monte Carlo-style performance testing
- Guidance parameter tuning and comparison
- 3D trajectory visualization
- Simulation dashboard for configuration and analysis

## Results

### Overall Performance

**~91% successful intercept rate**

**32,980 randomized engagement scenarios**

The batch-testing framework was used to evaluate guidance performance across
a large range of engagement conditions rather than relying on individual
hand-selected scenarios.

Detailed outputs and plots are available in the [`results/`](results/) folder.

## Simulation Examples

Example outputs from individual simulation runs and the simulation interface
are available in the [`demos/`](demos/) folder.

These demonstrate the interceptor and target trajectories, guidance behavior,
obstacle interaction, and engagement visualization.

## Guidance Tuning

Guidance parameters were evaluated across repeated engagements to identify
combinations that produced stronger overall intercept performance.

The resulting tuning heatmap and batch-test outputs are available in the
[`results/`](results/) folder.

## Repository Structure

```text
Guidance-and-Intercept-Simulation/
│
├── README.md
│
├── src/
│   └── MATLAB simulation source code
│
├── results/
│   └── Batch results, trajectory plots, and tuning analysis
│
└── demos/
    └── Live simulation and dashboard examples
