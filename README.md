# primary_structure_pl_001
primary_structure_pl_001
## Contents
* Introduction
* Setting up conda environment
* Runnibg training experiemnt

### Introduction
This is a guide to running a bioinforatics pipline that calculaes disecrptors that describe the change in physical properties in primary amino acid struture upon a mutationin genomic DNA. The input strutures are tripeptides, of the structur Gly-X-Gly or GXG, for example Gly-Ala-Gly or GAG. There are enrgy minimised struture and 50 ns molecular dynamics simulations availible for the X equals the twenty edogenous amino acids. 

### Setting up conda environment
We set up the conda encironment, I am including instruction of how I do this, later we may one to clone the envirnomant, ```conda create -n pri_struc_pl_001  python=3.10```, we activate our conda environment ```conda activate pri_struc_pl_001```. Next we install NWChem
NWChem instaltion via conda was installed using https://github.com/conda-forge/nwchem-feedstock.

```
conda config --add channels conda-forge
conda config --set channel_priority strict
conda install nwchem
```
To test that NWChem is install I ran standrad simulation of N2 using the ```n2.nw``` file and the command ```nohup nwchem n2.nw &``` output text is sent to nohup.out.

```conda install -c conda-forge xmlvalidator cmlgenerator nwchemcmlutils ssipfootprint phasexmlcreator phasexmlparser resultsanalysis puresolventinformation solventmapcreator phasecalculator```

