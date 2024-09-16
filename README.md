# URBAG_LCA_tool
URBAG python tool for the Metropolitan Area of Barcelona case study implementation.

# Documentation
The documention is currently under revision. Please contact gara.villalba@uab.cat for more information.

# Objective
A python tool to calcualte a prospective-regionalized LCA of peri-UA areas detailed in a map potentially comparing circular and linear sources of nutrients, as well as water requirements and impacts.

# Requirements
Python 3.11 or 3.12
License for ecoinvent 3. Please note that the ecoinvent database is not included in this package. Also, read ecoinvent's GDPR & EULA.
Map of peri-UA areas.
Emission factors for circular and linear products (default provided).
Footprints of impacts of circular products (the ones provided are for the Metropolitan Area of Barcelona only).

# How to use it?
1. Download the zip. 
2. Check all notebooks for the choice of scenario under the scen variable. Where you find the following text:
    #In this cell the scenario is chosen. This can either be defined here or in the RUN_ALL.ipynb
    #If defined here unmark the scen = line and select the scenario you will run.
    #If defined in RUN_ALL.ipynb unmark the %store -r scen line and remark the scen = line.
    #Scenario names are:
    #S0_MinFert > N,P,K demand met by mineral fertilizers only
    #S0_struvite_P > P demand met by struvite, N demand met by struvite and mineral fertilizer and K demand met by mineral fertilizer
    #S0_compost > N,P,K supplied by compost produced in the AMB, remaining N,P,K demand met by mineral fertilizer
    #S0_Ammon_salts > N supplied from recovered ammonium salts and from mineral fertilizers, P from struvite and K from mineral fertilizer
    scen = 'S0_MinFert'
    #%store -r scen
Select the right option for you.
3. In the inputs folder find the file URBAG_LCIAs_ei391cutoff_20240409.xlsx and change the dummy numbers (ones in yellow highlighted cells) for the real mineral fertilizer footprints. 
To reproduce our study we used ecoinvent v3.9.1. for indicated processes for mineral fertilizers.
4. If you choose RUN_ALL.ipynb, select one scenario in this Notebook and run all cells.
5. If you choose to run each notebook independently, run them in numerical order from 0 to 8_2.
Results should be reported in the output folder for each scenario selected.

# Support
gara.villalba@uab.cat

# Contributors
Angelica Mendoza Beltran.
Gara Villalba.
Erin Untereiner.  

# References
Under development. 

# License
CC BY-NC-SA. Attribution-NonCommercial-ShareAlike 4.0 International. https://creativecommons.org/licenses/by-nc-sa/4.0/
