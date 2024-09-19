# TreeSwallow_TelomereAndCalcium
Reproductive output and telomere dynamics following calcium supplementation in wild Tree Swallows (Tachycineta bicolor)

This data is the result of an experiment investigating whether biologically relevant differences in reproductive investment influence telomere length in a wild bird species. We employed calcium supplementation to experimentally modify reproductive output in Tree Swallow mothers and offspring and we used telomere dynamics during the breeding season as a proxy for stress associated with reproduction. To confirm that calcium supplementation positively impacts reproductive parameters at our study site, we initiated a 4-year trial of calcium supplementation with our Tree Swallow study population. In the following two breeding seasons, we used calcium supplementation to experimentally alter reproductive output and measured telomere length in mothers immediately before egg-laying and shortly before fledging to determine the direct relationship between reproductive investment and telomere shortening in this species. Our study includes one hundred eighty-eight nests initiated and monitored over six breeding seasons. 


## Description of the data and file structure

The "calcium_supp.csv" document includes data from the experiment confirming that calcium supplementation positively impacts Tree Swallow reproductive parameters. The "TRT" column indicates whether the nest received the calcium supplement (crushed oyster shell) or the treatment (local soil). The "Clutch" column indicates clutch size, which is the number of eggs that the mother laid. The "Hatch" column indicates the hatching success of the nest, which is the proportion of eggs hatched out of the number laid. The "Year" column is the year the data was collected. The "Volume" column is the mean egg volume (in mm) of the nest, calculated using the formula V=0.51LW2, where L is the length of the egg, W is the width of the egg, and 0.51 is a species-specific constant. Cells with an "NA" indicate data was not able to be collected for the respective measurement.

The "TL_moms.csv" document includes data from the experiment measuring telomere shortening in mother Tree Swallows following calcium supplementation. The "ID" column includes the ID of the mother Tree Swallow. "TL_pre" is the standardized relative telomere length of the mother before breeding, while "TL_post" is the standardized relative telomere length of the mother post-breeding when chicks were 12 days old. The "Age" column classifies the mothers into two age classes; SY is "second-year" which means the bird is a one-year old (this is the birds second summer, inluding the summer it was born). ASY is "after second-year" which means the bird is older than one year. The "TRT" column indicates if the nest recieved a calcium or controld treatment. "Year" indicates the year the data was collected. The "Clutch" column indicates clutch size, which is the number of eggs that the mother laid.The "Brood" column indicates how many chicks hatched from the nest. The "Hatch" column indicates hatching success, which is the number of eggs that hatched out of the number laid. Cells with an "NA" indicate data was not able to be collected for the respective measurement.

The "D" column is the measre of temporal telomere shortening adjusted for the regression to the mean, using the equation: 
```math

D = \rho(X_1 - \bar{X}_1) - (X_2 - \bar{X}_2), \text{ where }
```

```math
\rho = \frac{2r s_1 s_2}{s_1^2 + s_2^2}, \text{ where }
```
X1 is the RTL for mothers at time-point one (pre-breeding), X2 is the RTL for mothers at time-point two (when chicks were 12 days-old), r is the correlation between X1 and X2, s is standard deviation, and s2 is variance. 

The "TL_chicks.csv" document includes data from the experiment measuring average telomere length of chicks in a nest following calcium supplementation.The "NestID" column indicates the ID given to each nest box. "NestTL" indicates the average telomere length of each nest. "MomTL" indicates the telomere length of the mother pre-breeding. The "Treatment" column indicates whether the nest recieved the calcium or control treatment. "MomAge" gives the age classification of the mother Tree Swallow. "Year" indicates the year the data was collected.
