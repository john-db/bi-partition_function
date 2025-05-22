# Real Data Analysis

This folder contains two Excel files:  
- `bip_func_before_corrections.xlsx`  
- `bip_func_after_corrections.xlsx`  

These files contain the values of the bi-partition function for the trees visualized in `tree_before_corrections.pdf` and `tree_after_corrections.pdf` (also included in this folder), respectively.

For each tree, the bi-partition function has been computed for each mutation and the clade it seeds. Each clade is represented as a separate worksheet in the corresponding Excel file.

**Worksheet Naming Convention**  
Please note that Excel imposes a limit on worksheet name length. As a result, each worksheet (i.e., clade) is named using the following format:  
- The name starts with the leftmost cell in the clade (as seen in the drawing of the corresponding tree),  
- followed by `..`,  
- and ends with the rightmost subline contained within the clade (also determined as seen in the drawing of the corresponding tree).

Although these names are generally sufficient to identify each clade, an additional column is provided within each worksheet that explicitly lists all sublines included in the clade.

---

For details on tree inference and the input data (including the noisy genotype matrices used to run the bi-partition function algorithm), please refer to the following repository:
🔗 [https://github.com/smalikic/Tree-Inference/tree/main](https://github.com/smalikic/Tree-Inference/tree/main)
