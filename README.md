# Warehouse Automation Simulation

## Project Overview

The Warehouse Automation Simulation project models an advanced automated manufacturing system using discrete-event simulation in Python. This system integrates multiple subsystems, including a Manufacturing Preparation Center (MPC), an Automated Guided Vehicle (AGV) fleet, and a Work Center. The objective is to evaluate system performance, optimize throughput, and analyze different system configurations.

## System Components

1. **Manufacturing Preparation Center (MPC)**
   - Operators process raw materials into fixtures.
   - A joint buffer stores prepared fixtures before transportation.
   - Workstations facilitate operator efficiency.

2. **Automated Guided Vehicles (AGV) Fleet**
   - AGVs transport fixtures between the MPC and the Work Center.
   - Dynamic task allocation minimizes idle time and optimizes flow.
   - Battery management ensures continuous operation.

3. **Work Center**
   - Milling machines process fixtures.
   - Internal buffers store fixtures before and after processing.
   - A robotic system transfers fixtures between buffers and the loading dock.

## Objectives

- Develop modular simulation models for each subsystem.
- Validate simulation results using analytical methods.
- Investigate alternative system configurations to improve efficiency.

## Simulation Scenarios

### 1. **Baseline System Performance**
   - Evaluate throughput and flow time using the default configuration.
   - Identify potential bottlenecks in material flow and machine utilization.

### 2. **AGV Fleet Optimization**
   - Implement dynamic AGV selection based on workload.
   - Model battery recharging behavior and its impact on system performance.

### 3. **Operator and Shift Management**
   - Simulate operator shift breaks and bio breaks to understand their impact.
   - Compare different staffing levels and break schedules.

### 4. **System Configuration Variations**
   - Analyze the impact of increasing the number of machines, AGVs, and workstations.
   - Optimize buffer sizes for reduced wait times and improved efficiency.

## Implementation Details

- **Simulation Framework:** Python with SimPy for discrete-event simulation.
- **Key Metrics:** Throughput, flow time, machine utilization, AGV efficiency.
- **Validation Approach:** Analytical modeling and multi-run simulation comparisons.

## Running the Simulation

1. Clone the repository:
   ```sh
   git clone https://github.com/Warehouse-Automation/warehouse-automation.git
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the main simulation script:
   ```sh
   python simulation.py
   ```
4. View results and analysis in the generated reports.

## Future Enhancements

- Introduce traffic congestion modeling for AGVs.
- Implement machine failures and maintenance schedules.
- Develop a real-time dashboard for visualization.

## Contributors
- Álvaro Arrieta Puente
- Vasileios Karvouniaris
- Milly Landmeter
- Ioanna Panagiotopoulou
- Kars Polderman
- Paulo Vieira

 ```
```
 

