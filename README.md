# Prosperdyn
Describe Dynamics in Prospective Life Cycle Assessment

- Independent modification of background and foreground data for streamlined scenario modelling of time-differentiated life cycle inventories.
- Approach an environmental target by defining industrial transition paths in the foreground data.

Background data for each time step can be imported using [premise](https://github.com/polca/premise). Foreground data can be created for each time step absolutely or using relative information, which must be defined simultaneously. Data for the required novel infrastructure can be calculated in a coupled separate inventory. Inventory calculations are carried out using methods from [brightway2](https://github.com/brightway-lca/brightway2). Also arbitrary static impact categories can be applied. Foreground scenarios can be modified successively in short time while background data remains unchanged.

The time-differentiated inventory results can be used for dynamic impact assessment by calculating the additional radiative forcing from greenhouse gas emissions.

All details are discussed in the following publication:
Lang-Quantzendorff, L., Beermann, M.: Prosperdyn—–a tool to describe dynamic transitions in prospective life cycle assessment. Int J Life Cycle Assess, (2025) 
[DOI: 10.1007/s11367-025-02515-x](https://doi.org/10.1007/s11367-025-02515-x)

The example presented in the journal article can be analysed in the following Jupyter Notebooks:
1. prosperData defines new dynamic foreground inventories with modified parameters.
2. prosperInvent calculates the demand for infrastructure and carries out dynamic inventory calculations and static impact assessments.
3. prosperImpact calculates the additional radiative forcing for dynamic impact assessment.
4. The environment premise_2 includes besides premise also [bw2analyzer](https://github.com/conda-forge/bw2analyzer-feedstock)
