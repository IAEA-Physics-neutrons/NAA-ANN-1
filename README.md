The objective of this code is to develop an Artificial Neural Network for analysis of Neutron Activation Analysis data.
This has been developed in 2022 for one simple specific case, as a proof of concept. A scientific paper is in preparation where full details will be given.
This contains two sets of code:
- A set of fortran routines for data augmentation. This is in file <NAA2 data augmentation source project 2022-04-27.zip>, which also includes the project files for the Intel Fortran Visual Studio Project.
- The data augmentation routine works on the data provided in the file <RID data 2022-04-27.zip>, which includes the original 216 real gamma spectra collected at the Research Institutt Delft, Netherlands, that constitute the simple specific example dealt with here. It also includes one txt file with file names and other parameters.
- The output of the data augmentation routine is in file <NAA2 data augmentation output 4e.zip>. The options with which the routine was ran are given in the file <4e_options.txt> contained in that zip.
- A jupyter notebook for the ANN. It uses Pandas, Numpy and Tensorflow libraries, given in file <NAA1 2022-05-09 4e>. It uses as input some of the files contained in <NAA2 data augmentation output 4e.zip>, namely <4e_data_iiiii.dat> and <4e_synth_iiiii.dat>, where iiiii is a five digit integer, <4e_in_data.csv> and <4e_in_synthetic.csv>.
- The output of the ANN, namely for the Selenium content, its uncertainty and limit of detection, for the training set and the test set, are given in the file <NAA1 2022-05-09 4e results.csv>. Note that the training process uses random numbers, and each run of the code will produce slightly different results.

- Different code versions and their output are now organized by date. If a code version and a data file version have the same date, they correspond to the same version.
