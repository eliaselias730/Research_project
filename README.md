Introduction of project
Driven by the urgency of meeting climate targets and the growing political focus on sustainability, the world is transitioning from fossil fuels to renewable energy. However, the inherent variability of these sources and geographical mismatches between supply and demand necessitate the development of efficient energy vectors or storage technologies, to ensure a reliable and continuous flow of energy. Hydrogen has gained increasing interest in fulfilling this role however safety concerns have forced development of alternatives energy carriers. Liquid organic hydrogen carriers (LOHCs) offer a safe and convenient solution for energy storage by chemically binding hydrogen to organic molecules in reversible hydrogenation and dehydrogenation cycles over catalysts. This approach enables safe long-term storage and handling of hydrogen at ambient conditions. 

The code models the dehydrogenation reaction of perhydro dibenzyltoluene (H18-DBT) to dibenzyltoluene (H0-DBT)
stoichiometry: H18-DBT --> H0-DBT +9H2

Plug flow reactor (PFR) model 
File - MATLAB code solving ODEs to find mass of catalyst required for defined conversion and pressure drop

Slurry model
The dehydrogenation unit was modelled as a horizontal flow reactor consisting of a slurry of catalyst and liquid reagents. Produced hydrogen was assumed to leave the system without influencing the residence time of the liquid phase in the reactor. The reaction kinetics are described with the same assumptions as in the kinetics section above. A cascade of 10 identical CSTRs (continuous stirred tank reactor) was used to approximate the reactor. The CSTRs are connect in series with the outlet conditions such as temperature and composition as input conditions for the next tank. Volume of liquid was assumed to be constant as the density of H18-DBT and H0-DBT are very similar and vapour content of LOHCs were assumed negligible. Perfect mixing is assumed therefore, no concentration and temperature gradients, no radial or axial heat transfer.

MATLAB file - This contains input variable to SIMULINK file containing the model. This file also extracts required data from the SIMULINK model. 
SIMULINK file - contains model
