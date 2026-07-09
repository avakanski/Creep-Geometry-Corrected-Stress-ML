# A Temperature-Dependent Geometry-Corrected Stress Descriptor for Machine Learning-based Prediction of Creep Rupture Life
**Authors: T. Wang, J.W. Merickel, Y. Tang, F. Xu, A. Vakanski, R. Song**

Accurate prediction of creep rupture life is essential for assessing the structural integrity and long-term reliability of high-temperature components in nuclear energy systems. However, creep rupture data obtained from specimens with different sizes and geometries exhibit variability that is not adequately addressed by conventional creep life methods or advanced predictive approaches. 

This study extends the fractal stress renormalization approach by incorporating characteristic specimen size, cross-sectional area, and aspect ratio, and introduces a temperature-dependent correction derived from dimensional analysis and incomplete self-similarity theory. The resulting geometry-corrected stress is employed for developing machine learning models by combining physically interpretable size correction with data-driven prediction. 

The framework was evaluated using a database comprising 2,433 creep tests from ten nuclear-grade structural materials, including austenitic stainless steels, reactor pressure vessel steels, nickel-based alloys, and zirconium alloys. The proposed correction significantly reduced geometry-induced scatter in stress-rupture life relationship. 

In machine learning evaluation, a gradient boosting model incorporating the temperature-dependent geometry-corrected stress achieved the highest predictive performance (R² = 0.9142), outperforming models based on nominal stress, direct inclusion of geometric variables, and conventional creep correlations. 

The results demonstrated that representing specimen geometry through a physics-informed stress descriptor improved creep rupture life prediction across diverse specimen geometries and nuclear structural materials.

## 📂 Repository Organization
- [**Dataset**](Dataset/): Contains the creep dataset used for model training, analytical correlation, and performance evaluation.
- [**Tables**](Tables/): Contains Jupyter notebooks for generating the tables reported in the study. Each notebook reproduces one table and displays it at the end of the notebook.
- [**Figures**](Figures/): Contains Jupyter notebooks for generating the figures reported in the study.

## 📊 Data
- [**Dataset**](Dataset/): The creep property dataset used in this study is associated with the article ***Compilation of Creep Property Data for Nuclear Structural Materials*** and is available at [https://doi.org/10.1038/s41597-026-07563-y](https://doi.org/10.1038/s41597-026-07563-y).
- The dataset file used by the notebooks is named: `Creep_Properties_Dataset.xlsx`.

## 🔨 Requirements
- pandas
- numpy
- scikit-learn
- scipy
- matplotlib
- openpyxl
- xgboost
- jupyter

## ▶️ Use
The reproducible code is provided as Jupyter notebook files in the `Tables` and `Figures` folders. Place `Creep_Properties_Dataset.xlsx` in the `Dataset` folder, then run the corresponding notebooks to generate the reported tables and figures.

## 🚩 License
<a href="LICENSE">MIT License</a>

## 👏 Acknowledgments
This work was supported through the INL Laboratory Directed Research & Development (LDRD) Program under DOE Idaho Operations Office Contract DE-AC07-05ID14517 (project tracking number 24A1081-149). Accordingly, the publisher, by accepting the article for publication, acknowledges that the U.S. Government retains a nonexclusive, paid-up, irrevocable, worldwide license to publish or reproduce the published form of this manuscript or allow others to do so, for U.S. Government purposes.

## ✉️ Contact or Questions
A. Vakanski, e-mail: vakanski@uidaho.edu  
R. Song, e-mail: Rongjie.Song@inl.gov
