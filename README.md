# Cyber-Physical System (CPS) Risk Assessment using Bayesian Networks (BN) and AutomationML

This repository provides resources and code for performing risk assessments of Cyber-Physical Systems (CPS) using Bayesian Networks (BNs) derived from Automation Mark-up Language (AutomationML) models. The BN structures capture probabilistic dependencies among CPS components, vulnerabilities, and hazards—enabling integrated assessment across cybersecurity, reliability, and safety dimensions.

The use of AutomationML, based on the CAEX (Computer Aided Engineering Exchange) schema, supports machine-readable and hierarchical representations of CPS assets and interdependencies. This facilitates model consistency, domain knowledge integration, and dynamic risk analysis.

This methodology builds upon the findings of Bhosale et al. (2024), available at:  
[https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10623880](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10623880)

---

## 📂 Repository Contents

### `AML_BN_CPS.py`  
Performs BN-based CPS risk assessment on a generic AML model. Computes probabilities of failure and system-level impact. Tested on Python 3.12.8.

### `AML_BN_Stuxnet.py`  
Applies the risk modelling framework to the Stuxnet cyber attack scenario. Parses `Stuxnet.aml` and generates BN outputs.

### `AML_BN_BlackEnergy.py`  
Implements BN-based analysis on the BlackEnergy malware attack scenario using the corresponding AutomationML file.

### `AML_BN_SolarPV.py`  
Demonstrates the methodology in a Solar PV attack context. Based on ForeScout’s SUN:DOWN research:  
[https://www.forescout.com/research-labs/sun-down-a-dark-side-to-solar-energy-grids/](https://www.forescout.com/research-labs/sun-down-a-dark-side-to-solar-energy-grids/)

### `AML_BN_CBTC.py`  
Analyses a railway Communication-Based Train Control (CBTC) attack scenario. Uses `RailwayCBTC.aml` to derive risk scores.

### `utils.py`  
Contains shared utility functions for AML file parsing and probability computation.

---

## 📁 AML Models

- `Generic_CPS.aml`: Canonical CPS configuration authored in AutomationML.
- `Stuxnet.aml`: Encodes assets and attack vectors observed in the Stuxnet case.
- `BlackEnergy.aml`: Captures structural elements and vulnerabilities from the BlackEnergy attack.
- `RailwayCBTC.aml`: Represents a CBTC-based railway cyber attack scenario.

---

## 📄 Bayesian Network Model

- `Generic_CPS_BNN.xdsl`: BN model of a generic CPS system, developed using GeNIe Academic v5.0.

---

Feel free to open an issue for questions, improvements, or scenario extensions.
