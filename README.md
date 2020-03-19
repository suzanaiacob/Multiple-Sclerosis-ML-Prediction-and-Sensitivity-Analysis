# Multiple Sclerosis ML Prediction and Sensitivity-Analysis

This is my MIT Project for the course Machine Learning Under a Modern Optimization Lens, taught by the Associate Dean for Business Analytics at MIT, Dr. Dimitris Bertsimas. This project was completed in collaboration with my MIT colleague El Ghali Ahmed Zerhouni. We submitted this for our final project and received a grade of A :) 

The project was open-ended, we were tasked with using any methods on any problem of our choice.

I am outlining here the overview of the files, for the project overview and conclusions, please read the project report and poster. The overall goals of this project are :
- To build ML models which **accurately predict which treatment to give to which patient**
- To employ novel ML techniques (that we develop here at MIT) - **Optimal Classification Trees**
- To develop a methodological approach to making ML models more **robust** (that is maintaining good results under changes in the underlying data)

## Project overview 
- **Project report**: Multiple Sclerosis - From Predictions To Sensitivity Analysis And Robust Models.pdf
- **Project poster**: Personalized treatment prediction for MultipleSclerosis.pdf

## Code files 
The code is half in R and half in Julia. In general the code can be run, but it requires an IAI licence: https://www.interpretable.ai/technology.html. To counter this, I am also publishing pdf versions of the Jupyter Notebooks, so the results can be viewed.

- data_exploration.rmd contains all the feature engineering steps this project required. 
- OCT_models containts the intials models and cross-validation
- CART_GLM_Sensitivity contains sensitivity analysis of CART Model and it's robustification throught generating a more robut training set. It also contains a multinomial lasso-regularized logistic model, trained both on the classic data set and the robust one.
- kmeans_presctiption contains the kmeans prescriptive algorithm and its sensitivity analysis
- OCT_GLM_robustification contains sensitivity analysis on=f three OCT models and their comparison with OCT-H and robustification. It also plots the perfomance of robust multinomial logistic regression as a comparison algorithm
- The file data contains the data we used


Data available from this study: https://bmcneurol.biomedcentral.com/articles/10.1186/s12883-015-0450-x 
