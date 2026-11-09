# Detecting Fake Measurement Data Attacks on SDN Controllers

COMP3000 Computing Project (2026/27)

| | |
|---|---|
| **Student** | Yang Chun Kit |
| **Supervisor** | [Supervisor name - to be added] |
| **Project management** | [Jira: backlog, sprints, timeline and sprint diary](https://simonyck-comp3000.atlassian.net/jira/software/projects/SCRUM/boards/1) |

## Project Vision

Software-Defined Networking (SDN) controllers use network statistics to make automated decisions, such as blocking suspicious traffic. However, manipulated measurements may cause incorrect decisions, including blocking legitimate hosts or failing to detect attacks.

This project aims to investigate how falsified measurement data affects SDN security decisions, and to develop and evaluate a controller-independent method to detect such manipulation.

## Research Questions

**RQ1:** How do manipulated traffic measurements affect automated SDN security decisions?

**RQ2:** Are these effects consistent across different SDN controllers?

**RQ3:** How effectively can cross-switch consistency checking detect falsified measurements, and what are its limitations, false-positive rate and performance overhead?

## Planned Approach

An isolated Mininet lab will run a threshold-based security application on Ryu and a second controller (ONOS or OpenDaylight). Two attack classes will be tested: falsified switch measurements and genuine but misleading traffic from end hosts. A detection module will receive flow statistics from each controller through adapters in a common format, and compare measurements from adjacent switches.

## Ethics

All attack code in this repository is for authorised academic research and is only run in an isolated virtual lab with no access to external or production networks.
