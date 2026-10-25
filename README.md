# Cyber-Physical Agent Orchestrator

An in-progress architecture concept for coordinating AI planning, knowledge retrieval, visual feedback and edge equipment execution.

**Company application:** I contribute to a server assembly application at my company.

## Concept

The orchestration concept connects task knowledge and spatial information with physical actions, then uses observations to revise the plan. Server assembly inspection is an example application; broader use across objects and equipment remains a development direction.

## Agent responsibilities

| Agent | Responsibility |
|---|---|
| Planner | Coordinate tasks, retrieve relevant knowledge and revise acquisition plans. |
| KM | Retrieve task specifications, relevant CAD geometry and prior observation knowledge. |
| Physical | Execute permitted camera and lighting actions at the edge and report equipment limits. |
| VLM | Analyze observations and return visual findings or optical feedback for replanning. |

## Feedback loop

Task and knowledge -> Plan -> Edge execution -> Visual observation -> Feedback -> Revised plan.

Cloud reasoning and edge execution are separated. Physical actions remain subject to local equipment limits. Interfaces, execution behavior and outcomes require implementation and validation.

## Example: server assembly inspection

An unclear image caused by reflection or shadow can prompt a revised lighting or capture plan before another observation.

![Server assembly example architecture](server-assembly-inspection-architecture.svg)

## Project status

Architecture concept in progress. The material illustrates a general orchestration approach; it does not establish a completed general-purpose 3D platform or measured production performance. Only generic concepts are included here.

[Download concept summary](case-study.pdf)
