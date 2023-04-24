# LBL binary electrolyte research

## Thermodynamic properties of electrolytes

Performance of electrolytes in Li-ion batteries is characterized by thermodynamic properties such as the activity coefficients of salts and solvents, thermodynamic factor of salts and the osmotic coefficient of solvents. Often, experimental data found in literature are only available in one thermodynamic property. Fortunately, there are equations you can use to convert between these properties. The code in conversions.ipynb contains 8 different functions that convert 4 different thermodynamic properties to each other.

## Molarity and Molality

xmc.ipynb shows converting between molality and molarity.

## Self-proposed mixing rules for activity coefficient of electrolytes

mixin-rules.ipynb presents four different functions representing four self-proposed mixing rules to predict the activity coefficient of single salts in binary solvents (e.g. LiPF6(salt) in 40%-Ethanol(solvent 1)-60%-water(solvent 2))

### Why are we interested in double solvents?

Using two solvents in practice is better than using only one pure solvent (getting the best of both worlds and negating the drawbacks of using a single pure solvent).

Most literature that deal with single salt-double solvent electrolytes presents activity coefficient data in terms of different ratios (e.g. pure ethanol, 1:9 ethanol:water, 2:8 ethanol:Water, and so on). However, some papers might not have data for some proportions that we want (e.g. we want to know the activity coefficient of 1:1 EC:EMC but papers only have pure EC and pure EMC data, or we want to know 4:6 EC:EMC but there's only data for 7:3 EC:EMC).

This repo contains 4 different mixing rules that predict the activity coefficient of mixed solvents from pure solvent values (or other proportions of mixed solvent values). The second mixing rule, the Mole Fraction Average, is the most accurate of the four when compared to existing literature data.
