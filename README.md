# thermochemical-data-fusion

List of files
=============

<br>1) smiles_to_graphs.py
<br>&emsp;    This file contains code to convert a list of smiles (read from a text file) to the data matrix.
<br>2) lasso_fits.py
<br>&emsp;    This file contains the LASSO implementation used in the paper.
<br>3) bootstrap_error_estimation.py
<br>&emsp;    This file can be used to generate a bootstrap sample of mean absolute error (MAE) for the model.
<br>4) helper_files.py
<br>&emsp;    This file contains a list of plotting helper functions used in the paper.
<br>5) model_details.json
<br>&emsp;    JSON file contains details of the three models (E-E, E-H and E-G) in the following pseudocode format:

<br>&emsp;'electronic energy': {
<br>&emsp;&emsp;	'coeff': list(ee_model.model_.coef_),
<br>&emsp;	'X_mean': list(ee_model.X_scaler.mean_),
<br>&emsp;	'X_std': list(ee_model.X_scaler.scale_),
<br>&emsp;	'y_mean': list(ee_model.y_scaler.mean_),
<br>&emsp;	'y_std': list(ee_model.y_scaler.scale_)},
<br>
<br>'enthalpy': {
<br>&emsp;	'coeff': list(eh_model.model_.coef_),
<br>&emsp;	'X_mean': list(eh_model.X_scaler.mean_),
<br>&emsp;	'X_std': list(eh_model.X_scaler.scale_),
<br>&emsp;	'y_mean': list(eh_model.y_scaler.mean_),
<br>&emsp;	'y_std': list(eh_model.y_scaler.scale_)},
<br>
<br>'free energy': 	{
<br>&emsp;	'coeff': list(eg_model.model_.coef_),
<br>&emsp;	'X_mean': list(eg_model.X_scaler.mean_),
<br>&emsp;	'X_std': list(eg_model.X_scaler.scale_),
<br>&emsp;	'y_mean': list(eg_model.y_scaler.mean_),
<br>&emsp;	'y_std': list(eg_model.y_scaler.scale_)}
</p>
