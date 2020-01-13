1. [for SNP visualization](http://www.vls3d.com/index.php/links/bioinformatics/mutations)
2. [Bioinformatics oneliners](https://github.com/stephenturner/oneliners)
3. [PandasPDB](https://rasbt.github.io/biopandas/tutorials/Working_with_PDB_Structures_in_DataFrames/)
# Generate random fasta.
```
x=0; while [ $x -le 50 ]; do R=$(echo ${RANDOM:2:2} | sed 's/0/1/'); echo '>'$(cat /dev/urandom | tr -dc 'a-zA-Z' | fold -w 32 | head -1)$(( x++ ))$'\n'$( shuf -zer -n${R}  {A,T,G,C} | tr -d '\0'); done
```
# Hail installation.
```
sudo apt-get install g++ liblz4-dev  
conda create -n hail python\>=3.6  
conda activate hail  
pip install hail  
conda install nb_conda  
conda install -c cyclus java-jdk  
```
