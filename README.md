# CO₂ Car Emissions Prediction  

## 📌 Project Overview  
This project builds **linear regression models in R** to predict car CO₂ emissions (grams/km) using the [Government of Canada’s Fuel Consumption dataset].
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
   - Identified strong correlations (e.g., CO2 vs fuel consumption: **0.935**).  

3. **Modeling**  
   - Built multiple regression models (stepwise, forward, backward, exhaustive search).  
   - Tested models with and without interaction terms.  
   - Compared Model 8 (interaction-based) vs. Model 9 (simplified).  

4. **Evaluation**  
   - Achieved high predictive accuracy (Adjusted R² ≈ **0.994**).  
   - Residual analysis confirmed improved variance stability after including interaction terms.  

## 🚀 Results  
- **Consumption, fuel type, year, transmission, and gears** emerged as the strongest predictors of CO2 emissions.  
- Model 9 provided a simpler structure while retaining high accuracy, making it effective for practical use.  
- Demonstrated that smaller models can still deliver reliable predictive performance.  

## 📂 Repository Structure  
```
├── Data/              # Raw and cleaned datasets (train/test splits)
├── Src/           # R scripts for analysis and modeling
├── Documentation/f   # Full project report
└── README.md          # Project documentation
```
