# R code

This folder contains the necessary R code to fit the shared component model used in the paper and the results obtained and the modified data to reproduce the results. The R software version used was R-3.5.2 and the R-INLA version 20.03.17.

The DataExample.txt contains the modified data. It contains the following variables:

-   Gender: Takes value 1 for males and 2 for females.

-   Age_group: Takes values 1 to 5 for age-groups 30-44, 45-59, 60-74, 75-89 and 90+.

-   Region_n: Takes the values 1 to 47.

-   Cancer: Takes value 1 for lung cancer and value 2 for LOCP cancer.

-   Cases: Observed number of deaths.

-   Population: Population.

-   i: a region index. Takes values 1 to 94. Note the model="besag2" defines a model with length $N=2n$ where $n$ is the size of the graph. In this case $2*47$.

-   i_P: take the value of 1 if the observation corresponds to lung cancer and 0 if the observation corresponds to LOCP cancer.

-   i_LOCP: take the value of 1 if the observation corresponds to LOCP cancer and 0 if the observation corresponds to lung cancer.

-   LOCP_het: take the value of the Region number (1 to 47) if the observation corresponds to LOCP cancer and NA if the observation corresponds to lung cancer.

The file esp_prov_nb.inla contains the information of the neighbourhood matrix.

The ZonificacionEspanaProv folder contains the cartography of Spain.

The Code.Rmd file allow you to adjust the age and gender-specific shared component model using INLA and reproduce the results obtained in the paper.
