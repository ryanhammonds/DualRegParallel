Breaks DR steps down and runs them in parallel using GNU parallel. Randomise step may be edited to run on SLURM.

# DualRegParallel

Need to make these variables command line options (ie DualRegParallel --jobs=29 --out= ...)

# Modify these variables 
JOBS=28
OUTPUT=groupICA.dr
ICA_MAPS=groupICA/melodic_IC
DES_NORM=--des_norm
LOG_DIR=groupICA.dr/log
INPUT=`cat input_files.txt`
dm=design.mat
dc=design.con

# Don't change these (only NPERM if you have reason to)
NPERM=5000
DESIGN="-d $dm -t $dc"
