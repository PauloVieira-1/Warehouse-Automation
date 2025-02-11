
# Reliability Analysis of a Block Diagram

## Overview
This repository contains reliability calculations for a given block diagram using two methods:
- **Decomposition Method**
- **Enumeration Method**

## Problem Statement
We analyze a block diagram where each component has a given reliability, and we determine the system's overall reliability using probabilistic techniques.

## Reliability Calculation
The system consists of five components with the following reliability values:
- **R1 = 0.8**
- **R2 = 0.9**
- **R3 = 0.8**
- **R4 = 0.9**
- **R5 = 0.9**

### Case I: Component 4 Fails
- Probability of failure = **1 - R4 = 0.1**
- **R_I = R1 * R2 * R3 = (0.8) * (0.9) * (0.8) = 0.576**

### Case II: Component 4 Does Not Fail
- Probability = **R4 = 0.9**
- **R_II = 1 - [(1 - R2 * R3) * (1 - R5)]**
  - **= 1 - [(1 - (0.9 * 0.8)) * (1 - 0.9)]**
  - **= 0.972**
- Final system reliability:
  - **R_sys = (1 - R4) * R_I + R4 * R_II**
  - **= (0.1 * 0.576) + (0.9 * 0.972) = 0.9324**

## Results
The system reliability is **0.9324** using the decomposition method.

## Usage
To reproduce the calculations, follow these steps:
1. Review the block diagram structure.
2. Apply probability rules to determine parallel and series system reliability.
3. Use the formulas above to compute the final reliability.

## References
- Ebeling, *An Introduction to Reliability and Maintainability Engineering*, 3rd ed.
- Reliability engineering principles and probability theory.
