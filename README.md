# urea_machine
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
| absorbances_dataset.csv | Spectra taken with UV-Vis spec for various urea concentrations in water and fresh dialysate  |
| absorbances.txt |    The .txt version of `absorbances_dataset.csv`   |
| nir_dataset.csv | Spectra taken with Cary5000 for various urea concentrations in saline |
| uvvis_absorbances_w_replicates.csv | Spectra taken with UV-Vis from 190-500 nm for urea in water with 3 replicates |
| pour_init.csv | Spectra taken with UV-Vis from 190-800 nm every hour during POUR from 9/14/2021 |

### Results
1. From data from UV-Vis from 190-500 nm for various urea concentrations in water with 3 replicates, PLS and PCA regression models were fit.  The wavelength range with the highest r-squared values for both regressions was determined.  For this dataset, the r-squared was 0.97 for both regression methods with an optimal wavelength range of 200-215 nm.
