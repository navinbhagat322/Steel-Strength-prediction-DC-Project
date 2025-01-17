# **Prediction of Mechanical Properties of Steels Using Machine Learning**  

## **Introduction**  
The mechanical properties of materials play a vital role in determining their behavior under applied loads. Characteristics like elastic modulus, strength, and ductility dictate how materials respond to stress, deflection, and eventual failure. Understanding these properties is essential since every mechanical system is subjected to loads during operation. Several factors influence mechanical properties, including microstructure, composition, heat treatment, and processing methods.  

Among these, composition and heat treatment are paramount, as they offer critical insights into the mechanical behavior of materials in various engineering applications. Traditional testing methods to evaluate these properties can often be time-consuming and expensive. Machine Learning (ML) has emerged as a promising alternative, enabling the prediction of material properties efficiently and cost-effectively.  

However, despite the growing adoption of ML in material science, there is no standardized methodology for systematically establishing composition-processing-structure-property relationships. This makes the exploration and prediction of such relationships a challenging task.  

---

## **Dataset Overview**  
The dataset used in this study, the **Fatigue Dataset for Steel**, was sourced from the **National Institute of Material Science (NIMS) MatNavi**. It is one of the most comprehensive databases available for analyzing material composition, processing parameters, and mechanical properties.  

### **Key Features of the Dataset**  
- **Chemical Composition:** %C, %Si, %Mn, %P, %S, %Ni, %Cr, %Cu, %Mo (all in wt.%).  
- **Upstream Processing Details:** Ingot size, reduction ratio, non-metallic inclusions.  
- **Heat Treatment Conditions:** Temperature, duration, and parameters for processes like normalizing, through-hardening, carburizing-quenching, and tempering.  
- **Mechanical Properties:** Yield Strength (YS), Ultimate Tensile Strength (UTS), %Elongation (%EL), %Reduction of Area (%RA), Hardness, Charpy impact value (J/cm²), and Fatigue Strength.  

### **Dataset Summary**  
- **Number of Instances:** 437 rows.  
- **Number of Features:** 25 composition and processing parameters.  
- **Target Variable:** Fatigue Strength.  
- **Steel Types Represented:**  
  - Carbon and Low-Alloy Steels: 371 instances.  
  - Carburizing Steels: 48 instances.  
  - Spring Steels: 18 instances.  

This dataset includes a variety of heats for each grade of steel under different processing conditions, providing a robust foundation for building predictive models.  

---

## **Methodology**  
1. **Data Preprocessing:**  
   - Cleaned and prepared the dataset for analysis.  
   - Standardized feature scaling to ensure uniformity across numerical data.  
   - Addressed missing values and ensured high-quality inputs for the models.  

2. **Feature Engineering:**  
   - Analyzed the importance of composition and heat treatment features.  
   - Identified key parameters affecting fatigue strength using exploratory data analysis (EDA).  

3. **Model Selection and Training:**  
   - Implemented machine learning models, including:  
     - Linear Regression.  
     - Decision Trees.  
     - Random Forest Regressor.  
     - Gradient Boosting Machines.  
   - Evaluated each model's performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² Score.  

4. **Prediction of Fatigue Strength:**  
   - Focused on understanding how compositional and processing variables impact fatigue strength predictions.  

5. **Validation:**  
   - Performed cross-validation to ensure robust and generalized model performance.  

---

## **Key Findings**  
1. **Feature Impact:**  
   - Heat treatment conditions and chemical composition were the most influential parameters in determining fatigue strength.  
   - Specific elements like %C (Carbon) and %Cr (Chromium) significantly influenced mechanical properties.  

2. **Model Performance:**  
   - Random Forest Regressor outperformed other models, achieving the best R² score and lowest error metrics.  
   - Ensemble methods demonstrated superior prediction accuracy compared to simpler models like Linear Regression.  

3. **Comparison with Experimental Data:**  
   - Predicted fatigue strength values closely matched experimental results, validating the efficacy of the machine learning approach.  

---

## **Conclusion and Future Scope**  
This study successfully demonstrated the potential of machine learning in predicting the mechanical properties of steels. By leveraging a robust dataset and advanced ML techniques, the project established key relationships between composition, processing parameters, and fatigue strength.  

### **Future Work:**  
1. Expand the dataset to include other steel grades and mechanical properties.  
2. Incorporate advanced ML techniques such as neural networks for improved prediction accuracy.  
3. Develop a user-friendly interface or dashboard for real-time fatigue strength predictions.  

This work paves the way for integrating AI and ML into materials science, offering a faster and cost-effective alternative to traditional testing methods.  
