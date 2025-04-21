# IRRBB Python Simulation

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)

A Python-based simulation for **Interest Rate Risk in the Banking Book (IRRBB)**, calculating **Repricing Gap**, **Economic Value of Equity (EVE)**, and **Net Interest Income (NII)** under the six EBA-prescribed interest rate shock scenarios (Parallel Up/Down, Steepener, Flattener, Short Rates Up/Down). This project demonstrates practical Asset and Liability Management (ALM) analytics, aligned with regulatory frameworks like **OSFI B-12** and **EBA IRRBB guidelines**, suitable for banking book risk management and regulatory reporting.

## Purpose
This repository provides a streamlined IRRBB simulation to model interest rate risk in a simplified banking book, supporting:
- **Regulatory Compliance**: Stress testing for EVE and NII under EBA scenarios, applicable to OSFI B-12 requirements for Canadian banks.
- **Data-Driven ALM**: Automation of risk metrics using Python, with outputs compatible with tools like Power BI for executive reporting.
- **Professional Development**: A practical project for professionals pursuing ALM certifications (e.g., PRMIA MLARM) or roles in banking risk management, showcasing data science and financial modeling skills.

Developed to align with modern ALM functions, this simulation emphasizes scalability, regulatory alignment, and integration with data analytics workflows.

## Features
- **Banking Book Modeling**: Simulates a portfolio with fixed-rate loans, floating-rate loans, floating-rate deposits, and non-interest-bearing demand deposits.
- **Gap Analysis**: Calculates repricing gaps in time buckets (3 months, 5 years) to assess interest rate mismatch risk.
- **EVE Calculation**: Computes the present value of assets and liabilities, discounted under base and shocked yield curves.
- **NII Estimation**: Models 1-year net interest income, adjusting for variable-rate repricing under shock scenarios.
- **Stress Testing**: Implements six EBA shock scenarios:
  - Parallel Up (+200 bps)
  - Parallel Down (-200 bps, floored at 0%)
  - Steepener (short -100 bps, long +100 bps)
  - Flattener (short +100 bps, long -100 bps)
  - Short Rates Up (+250 bps)
  - Short Rates Down (-250 bps, floored at 0%)
- **Dynamic Output**: Generates a dataframe report with **ΔEVE** and **ΔNII** (absolute and % of Tier 1 Capital) for regulatory and executive reporting.

## Installation

### Prerequisites
- **Python 3.8+**
- Required libraries: `pandas`, `numpy`

### Setup
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/jliu2025/irrbb-python-simulation.git
   cd irrbb-python-simulation
