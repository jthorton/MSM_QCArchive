# MSM_QCArchive
Calculating Modified Seminario Method Bond and Angle parameters from QCArchive

This notebook shows how to collect and process hessians from QCArchive to calculate new bespoke bond and angle molecular mechanics parameters for each molecule using the 
modified Seminario Method (https://doi.org/10.1021/acs.jctc.7b00785) as implimented in QUBEKit (https://github.com/qubekit/QUBEKit) (https://pubs.acs.org/doi/10.1021/acs.jcim.8b00767).

The parameters are then grouped by their associated smirks pattern and the mean and std values are calculated and ploted and compared against the values in taken from Openff-1.3.0.
A new custom Openff offxml is then made with the bond and angle equilibrium values and force constants taken as the average values from the modified Seminario Method.


## Requirements
* qubekit master
* openff-qcsubmit master
* openff-toolkit-base conda-forge
* rdkit conda-forge
