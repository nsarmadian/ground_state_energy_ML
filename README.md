# ground_state_energy_ML
ML on ground DFT calculated state energy of molecules
About Dataset
can be found in:
https://www.kaggle.com/datasets/burakhmmtgl/energy-molecule
This dataset contains ground state energies of 16,242 molecules calculated by quantum mechanical simulations.
It contains 1277 columns. The first 1275 columns are entries in the Coulomb matrix that act as molecular features. 
The 1276th column is the Pubchem Id where the molecular structures are obtained. 
The 1277th column is the atomization energy calculated by simulations using the Quantum Espresso package.
The first column (X1) is the data index and unused.

Past Research
The data is used for a publication in Journal of Chemical Physics. 
A blog post was also published explaining the data and the research behind it in less technical terms.

A Github repository is available that contains the source code used for generating the data, 
as well as some of the R scripts used for analysis.

Inspiration
Simulations of molecular properties are computationally expensive. 
The purpose of this project is to use machine learning methods to come up with a model 
that can predict molecular properties from a database of simulations. 
If this can be done with high accuracy, properties of new molecules can be calculated using the trained model. 
This could open up many possibilities in computational design and discovery of molecules, compounds and new drugs.
The purpose is to use the 1275 molecular features to predict the atomization energy. 
This is a regression problem so mean squared error is minimized during training.
