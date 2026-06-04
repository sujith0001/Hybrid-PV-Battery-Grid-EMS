# Hybrid-PV-Battery-Grid-EMS

Project Description
This project presents a Hybrid PV-Battery-Grid Energy Management System (EMS) designed and simulated in MATLAB/Simulink. The system integrates solar photovoltaic (PV) generation, battery energy storage, and utility grid supply to provide uninterrupted power to the load. An SOC-based controller intelligently manages source selection through breaker operation.

Features
Solar PV power generation model
Battery energy storage system
Utility grid backup source
State of Charge (SOC) based energy management
Automatic source switching using breakers
Voltage and current monitoring
MATLAB Function based EMS controller
Real-time visualization through Simulink scopes

System Operation
Mode 1: Solar Supply
When solar irradiance is available, the PV system supplies power to the load.
Mode 2: Battery Supply
When PV generation becomes insufficient and battery SOC is above the threshold level, the battery supplies power.
Mode 3: Grid Supply
When battery SOC falls below the specified threshold, the EMS disconnects the battery and transfers the load to the utility grid.

Simulink Components
PV Array Block
Battery Block
Utility Grid Source
Circuit Breakers (B1, B2, B3)
MATLAB Function Block (SOC Controller)
Voltage Measurement Block
Current Measurement Block
Resistive Load
PowerGUI Block

Simulation Parameters
Parameter
Value
Solar Irradiance
800 W/m²
Temperature
25°C
Initial SOC
30%
Solver Type
Discrete
Sample Time
5e-06 s

Results
The simulation demonstrates successful energy management among PV, battery, and grid sources.

Voltage Response
The load voltage remained nearly constant around 242.8 V, indicating stable system operation.

Current Response
The load current remained approximately 12.14 A with only minor variations, confirming reliable power delivery.

Breaker Operation
The EMS correctly activated the corresponding breaker based on SOC conditions and source availability.

Conclusion
The proposed Hybrid PV-Battery-Grid EMS successfully manages power flow between renewable and conventional energy sources. The SOC-based control strategy ensures uninterrupted supply while maximizing renewable energy utilization and protecting battery health.

Software Used
MATLAB
Simulink
Simscape Electrical
PowerGUI
