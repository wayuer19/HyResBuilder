# HyresBuilder: A simple package for building HyRes model.   
This package is forked from [PeptideBuilder](https://github.com/clauswilke/PeptideBuilder) and we do some modifications for HyRes.   
Thanks for the contribution of PeptideBuilder.    
Shanlong Li    

## Installation: 
git clone https://github.com/wayuer19/HyresBuilder.git   
python setup.py install


## Basic usage:   
This package builds HyRes peptide structure from sequence.    
### for a single sequence:   
Take tdp_43 as an example, to create HyRes tdp_43, one can just run:   
`python simple_example.py tdp-43-lcd.seq tdp-43_hyres.pdb`   
Please see the [examples](examples) for details.   

### for a set of sequence:   
To quickly build a series of peptides, one can run:   
`python bactch_example.py idps.seq`   
the first line in idps.seq gives the peptide names (also used as the pdb file name), and then the sequence in one line.   


To obtain psf file and further run simulation on OpenMM, please follow these [instructions](https://github.com/wayuer19/HyRes_GPU).   
>[!NOTE]
>After obtaining the pdb files, the initial structures need to be relaxed to get more reasonable state.   
  
## Modules:  
Module 1: HyresBuilder  
  build Hyres protein model  

Module 2: RNAbuilder  
  build RNA CG model

Module 3: HyresFF  
  create hyres system in OpenMM
