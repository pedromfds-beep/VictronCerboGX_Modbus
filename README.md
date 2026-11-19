# VictronCerboGX_Modbus
This Python script is a desktop GUI application designed for laboratory data acquisition, real-time monitoring, and control of energy storage systems (ESS). It acts as a central dashboard that interfaces simultaneously with Victron energy hardware (via a CerboGX controller) and laboratory measurement instruments (Keysight data acquisition units).
Key Features and Capabilities:
-- Victron CerboGX Integration (Modbus TCP)
Connects over Modbus TCP to read system parameters, battery states, inverter status, and power metrics across multiple slave IDs. Aggregates input power, output power, and AC consumption metrics.Monitors critical warning and alarm registers.
-- Keysight Instrument Integration (PyVISA)
Communicates with Keysight equipment (such as a 34972A data acquisition/switch unit) to scan channels and acquire analog measurements.Measures temperatures, auxiliary voltages, and calculates battery current based on user-defined shunt resistance.
-- Live Visualization & Plotting
Features a dynamic, multi-subplot live graph using matplotlib to track State of Charge (SoC), voltage, and current simultaneously during experiments.
-- ESS Power Control & Register Writing
Provides a dedicated control module to set and continuously stream Energy Storage System (ESS) power setpoints.Allows users to interactively view, edit, and write values to writable Modbus registers directly from the table interface.
--Data Logging
Includes options to log and export all acquired timestamped data streams into a structured CSV file for post-processing and analysis.
