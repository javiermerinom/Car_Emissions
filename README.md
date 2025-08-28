# CO₂ Car Emissions Prediction  

## 🏗️ Project Context
This was a research project developed for the second term of the Post-Degree Diploma in Data Analytics in Langara College.

## 📌 Project Overview  
This project builds **linear regression models in R** to predict car CO₂ emissions (grams/km) using the Government of Canada’s Fuel Consumption dataset.
The analysis includes descriptive statistics, feature evaluation, and regression modeling to identify the best predictors of emissions and compare model performance.  

## 🎯 Objective  
- Analyze fuel consumption, engine size, cylinders, transmission type, and fuel type to understand their relationship with CO₂ emissions.  
- Develop regression models to predict emissions and assess their accuracy.  
- Compare stepwise, forward, backward, and subset selection methods to optimize the model.  

## 🛠 Tools & Technologies  
- **Language:** R  
- **Libraries:** `MASS`, `leaps`, `ggplot2`, `dplyr`  
- **Techniques:** Stepwise regression, subset selection, interaction effects, model validation  

## 📊 Key Steps  
1. **Data Preparation**  
   - Cleaned and filtered the Government of Canada dataset.  
   - Split into training (80\%) and testing (20\%) sets.  

2. **Descriptive Analysis**  
   - Explored numerical (engine size, cylinders, consumption) and categorical (fuel type, transmission, class, gears) variables.  
   - Identified strong correlations (e.g., CO₂ vs fuel consumption: **0.935**).  

3. **Modeling**  
   - Built multiple regression models (stepwise, forward, backward, exhaustive search).  
   - Tested in total 9 models with and without interaction terms.
   - Compared Model number 8 (full model) vs. Model number 9 (reduced model).  

4. **Evaluation**  
   - Achieved high predictive accuracy (Adjusted R² ≈ **0.994**).  
   - Residual analysis confirmed improved variance stability after including interaction terms.  

## 🚀 Results  
- Full model (Model 8) comprised by **consumption, fuel type, year, gears, transmission, engine and interatction (consumption*fuel)** emerged as the strongest predictors of CO₂ emissions **(RMSE=1.83, R2=0.9992)**.  
- Reduced model (Model 9) comprised by **consumption, fuel type and its interaction** provided a simpler structure while retaining high accuracy **(RMSE=2.47, R2=0.9985)**, making it the most effective for practical use.  
- Demonstrated that smaller models can still deliver reliable predictive performance.  

## 📂 Repository Structure  
```
├── Data/              # Raw and cleaned datasets (train/test splits)
├── Src/           # R scripts for analysis and modelling
├── Documentation/f   # Full project report
└── README.md          # Project documentation
```
