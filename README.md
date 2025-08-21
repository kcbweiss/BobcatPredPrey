# Code to assess how prey availability impacts prey consumption using camera trap and scat data
R Code for assessing the overlap between predator and prey species in space and time and relative to predator diets

The following code utilizes the following steps:
1. Using assymmetric species interaction models (Richmond et al. 2010: DOI:10.2307/25741366) to calculate psiAB, or the probability that the Species A (predator) and Species B (prey) overlap in a given area. For our purposes, we did this in both wildland and exurban areas (spatial availability code)
2. Calculaing the activity overlap of the predator and each prey species (temporal availability code)
3. Running simulations where the value from steps 1 and 2 are multiplied together, while incoporating their respective error estimates (spatio-temporal availability code)
4. Running logit regression models to assess which model of availability (in space, time, or space/time) best predicts prey consumption, as defined via the frequency of scats that contain prey remains in the same study areas. Note: logit regression used, since scat values are constrained between 0-1 (0%-100% of scats) (Logit Linear Models Code)
5. Running Pearson's correlations to assess the relationship between prey consumption and prey availability

Note: Jesse Lewis (ASU) and Austin Green (Sageland Collaborative and University of Utah) helped with various aspects of the presented code

