# Non-functional Property Coupling

From the paper, _Exploring Non-functional Coupling in Systems of Systems_

Abstract:

> Many software systems, and especially systems of systems (SoS),
> depend on other systems to function correctly or are themselves
> composed of interdependent subsystems. In that context, behav-
> ioral changes in a dependency may have consequences for a depen-
> dent system. This includes changes to non-functional properties
> such as latency or availability. In this paper we use the term non-
> functional coupling to mean the extent to which a system is affected
> by changes to non-functional properties in other systems. We argue
> that non-functional coupling has implications for the reliability and
> performance of an overall system, as (for example) degradations in
> non-functional properties of one subsystem may cascade to other
> subsystems if coupling is high. In this paper we propose a process
> for systematically analyzing the coupling in a model of an SoS and
> illustrate that process with a simple case study showing how it can
> provide insights into system behavior, and how those insights can
> help with design decisions.

This repository contains the Quartermaster implementation of the proposed analytic process and the model and source code for the case study.

## Data

Includes summarized raw data from simulating the four models: original, A, B, C. The complete raw data, which includes more than the selected six non-functional properties can be recomputed by running the model.

## Quartermaster Model

Includes the Quartermaster source code for the case study model, including an entry point designed to run on a cluster.

## Visualization

The Python scripts used to

- generate the input parameters for each simulation
- read the raw simulation output data and create a scatter plot matrix
- perform a variance-based sensitivity analysis to generate the `coupling metric`
