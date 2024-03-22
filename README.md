# HyresBuilder: A simple package for building HyRes model.   
This package is forked from [PeptideBuilder](https://github.com/clauswilke/PeptideBuilder) and we do some modifications for HyRes.   
Thanks for the contribution of PeptideBuilder.    
Shanlong Li    

## Installation: 
git clone https://github.com/wayuer19/HyresBuilder.git   
python setup.py install


## Basic usage:   
This package builds HyRes peptide structure from sequence. Please see the [examples](examples) for details.   
To obtain psf file and further run simulation on OpenMM, please follow these [instructions](https://github.com/wayuer19/HyRes_GPU).   
>[!NOTE]
>After obtaining the pdb files, the initial structures need to be relaxed to get more reasonable state.   

Module 1: HyresBuilder  
  build Hyres protein model  


Module 2: RNAbuilder  
  build RNA CG model

Module 3: HyresFF  
  create hyres system for OpenMM
