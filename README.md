## Study of Dark Matter Production Models in the CMS Experiment at the LHC

This repository contains the analysis framework developed for the study of Dark Matter (DM) production models, focusing on vector and scalar mediator scenarios within proton-proton collisions at the LHC. 

The project focuses on the interpretation of CMS experiment data, processing Monte Carlo simulation samples to distinguish potential Beyond the Standard Model ($BSM$) signals from dominant backgrounds, such as $Z \rightarrow \nu\nu$ and $W \rightarrow \ell\nu$ processes.

# Workflow

The workflow of the project is divided into three keys steps.

# 1. Monte Carlo Event Generation
The signal and background samples were generated using MadGraph5_aMC@NLO within a Linux environment on the LXPlus (CERN) cluster. The new Dark Matter Simplified Model was defined in this enviroment and Monte Carlo generations with the hadronization and showering processes to produce realistic event outputs in ROOT format were performed. Se estudiaron diversos eventos para estudiar como los cambios de las masas de las nuevas partículas afectan a la física que podría verse en CMS.

# 2. Branching Ratio Study ("BR.ipynb")

Tras la generación de los eventos se decidió que canal de decay de dark higgs estudiar según los resultados obtenidos en este script que fueron estudiados en detalle en la memoria.

# 3. Data Analysis and Backgorund Supression ("main.ipynb")

The core of the analysis focuses on the characterization of the dark sector signal and its differentiation from Standard Model processes. 

Initially, the script explores the kinematic distributions of the simulated events to understand how different mass configurations of the new particles impact observable variables, identifying which parameters, such as missing transverse energy ($E_{T}^{miss}$) or jet momentum ($p_{T}$), are most sensitive to changes in the dark sector mass spectrum. 

Subsequently, a detailed study of the relevant backgrounds is conducted to establish the expected noise levels within the signal region. 

Finally, the signal is isolated from the background by applying optimized selection cuts and utilizing various statistical indicators, such as signal significance ($S/\sqrt{B}$), to maximize the detection potential of the model.

# 4. Statistical Analysis ("HypotesisTest.ipynb")

The final stage of the project involves a rigorous statistical evaluation to determine the viability of the proposed dark matter models. Using the data processed in the previous steps, this script performs hypothesis testing by comparing the background-only hypothesis against the signal-plus-background scenario. The primary tool for this assessment is the $CL_{s}$ method (Modified Frequentist approach), which is used to derive exclusion limits at a 95% confidence level.

