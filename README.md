# urea_machine
<span style="color: red;">This README is horribly out-of-date.</span>
  
![image](https://cdi.washington.edu/wp-content/uploads/2018/05/CDI-color-700.png)

### Objective
Use optical absorbance spectra for urea in solvent (water, saline, fresh dialysate) to predict urea concentration.

### Methods
1. Collect optical absorbance data with UV-Vis spectrophotometer for various urea concentrations in various solvents (water, 0.15M NaCl saline, fresh dialysate)
2. Observe various multivariate analysis and classifier algorithms on their accuracy of prediction.
3. Use PCA regression and PLS comparison model from here: https://scikit-learn.org/stable/auto_examples/cross_decomposition/plot_pcr_vs_pls.html

### Datasets
| Filename   |      Contents      |
|:----------:|:-------------:|
| urea_saline_uvvis.csv | Absorbance of urea in saline, UV-Vis region measured with UV-Vis spectrophotometer|
| urea_saline_cary5000.csv | Absorbance of urea in saline, 190-2500 nm measured with Cary5000 |
| urea_saline_normalized_cary5000.csv | Absorbance of urea in saline, normalized, 190-2500 nm measured with Cary5000, normalized version of urea_saline_cary5000.csv |
| pour_saline_uvvis.csv | Absorbance of POUR samples in saline, UV-Vis region measured with UV-Vis spectrophotometer |
  
### Results
1. From data from UV-Vis from 190-500 nm for various urea concentrations in water with 3 replicates, PLS and PCA regression models were fit.  The wavelength range with the highest r-squared values for both regressions was determined.  For this dataset, the r-squared was 0.97 for both regression methods with an optimal wavelength range of 200-215 nm.
