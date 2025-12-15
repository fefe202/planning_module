# Planning Module - Intelligent Systems

This repository contains the coursework for the **Planning Module** of the **Intelligent Systems** course. It explores automated planning techniques using **PDDL (Planning Domain Definition Language)** and **ANML (Action Notation Modeling Language)**.

## Project Structure

The project is organized efficiently to separate domain definitions, problem files, and documentation:

- **`anml/`**: Contains ANML domain and problem specifications.
    - `robot.anml`: Domain and problem definition for a robot navigation and object manipulation scenario.
    - `car.anml`: Domain modeling a car system.
    - `painter.anml`: Domain modeling a painting robot or system.
- **`pddl/`**: Contains PDDL domain and problem specifications.
    - `domain_robot.pddl`: The PDDL domain definition for the robot scenario (comparable to `robot.anml`).
    - `problem_robot.pddl`: The specific problem instance for the robot domain.
- **`docs/`**: Documentation and reports.
    - `report_benchmark.pdf`: A detailed report on the benchmarking results and analysis of the planning domains.
    - `Slides_ANML.pdf`: Presentation slides covering the ANML concepts used in this project.

## Domains Overview

### Robot Domain
A classic planning scenario where a robot must navigate between rooms, pick up objects (balls), and drop them at specific target locations. The domain handles constraints such as:
- **Movement**: Moving between connected rooms.
- **Battery**: Energy consumption for actions.
- **Carrying Capacity**: Limitations on what the robot can hold.

## Requirements

To run the planning problems in this repository, you will need compatible planners:

- **For PDDL**: Any standard PDDL planner (e.g., [Fast Downward](http://www.fast-downward.org/), [Metric-FF](https://fai.cs.uni-saarland.de/hoffmann/metric-ff.html)).
- **For ANML**: An ANML-capable planner (e.g., [FAPE](https://github.com/laas/fape) or other hierarchical task network planners that support ANML).

## Results

Detailed results of the planning definitions and their performance benchmarks can be found in `docs/report_benchmark.pdf`.
