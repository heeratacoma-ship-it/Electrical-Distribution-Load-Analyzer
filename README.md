# Electrical Distribution Load & Voltage-Drop Analyzer

Python-based electrical engineering project for analyzing voltage drop, conductor losses, and efficiency in a simplified multi-load 120 V distribution system.

## Features

- Models multiple electrical loads connected to a 120 V source
- Calculates branch current and delivered load voltage
- Calculates feeder voltage drop
- Calculates conductor power loss using I²R
- Calculates source power and load efficiency
- Evaluates multiple demand conditions
- Sweeps electrical demand from 50% to 180%
- Generates voltage-drop and power-loss plots using Matplotlib
- Exports calculated results to CSV

## Technologies

- Python
- Matplotlib
- CSV data export

## System Model

The program models three simplified loads:

- Lighting / Electronics
- General Load
- High-Demand Load

Each load is assigned a nominal power demand and feeder resistance.

The model evaluates how increasing electrical demand affects:

- Delivered voltage
- Current
- Voltage drop
- Feeder losses
- Efficiency

## Calculations

For each load, the program solves for delivered load voltage using the relationship:

```text
V_load² - V_source × V_load + P_load × R = 0
