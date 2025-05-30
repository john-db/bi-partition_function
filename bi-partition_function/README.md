Python implementation of the bi-partition function. To run the bi-partition function, run the file main.py using python:

python main.py -h

Required arguments:

-i : Path to input genotype matrix where rows correspond to cells/sublines and columns correspond to mutations. Please see example for format.

-c : Comma separated list of cells (row labels) to be used as the clade of interest for the partition function

-m : Mutation name (column label) to be used as the mutation of interest for the partition function

-n : Number of binary cell lineage tree topologies to be sampled

-fp : False-positive rate

-fn : False-negative rate

Optional arguments:

-s : Seed used for random number generation

Example: From the bi-partition_function directory execute:

python main.py -i example/data.tsv -c cell0,cell5,cell6,cell7,cell8,cell9,cell10,cell17 -m mut0 -n 100 -fp 0.01 -fn 0.1

The corresponding output is:

-----
elapsed time: 0:00:08.502752

Input: example/data.tsv

False-positive rate: 0.01

False-negative rate: 0.1

Clade: cell0,cell10,cell17,cell5,cell6,cell7,cell8,cell9

Mutation: mut0

Number of samples: 100

RNG seed: 0

numerator_est: 1.163944112761281013476341751E-41

denominator_est: 1.886298807317646730407156648E-39

Partition function estimate: 0.006170518203404009

-----
Indicating that mut0 has been estimated to have 0.6% probability of seeding the clade of cell0,cell5,cell6,cell7,cell8,cell9,cell10,cell17 by the partition function (with the small sample of 100 trees). In practice, we recommend sampling at least 1,000 trees.


