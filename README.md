# StatescopeData

## Available Cancer Signatures

| Tumor Type       | Number of Cell Types Available | Cell Types                 | Source           |
|------------------|--------------------------------|----------------------------|------------------|
| NSCLC            | 15                             |['Alveolar_cell', 'Monocyte', 'CD4_T_cell', 'B_cell', 'Plasma_cell', 'Fibroblast', 'Macrophage', 'NK_cell', 'CD8_T_cell', 'Neutrophil', 'Dendritic_cell', 'Endothelial_cell', 'Tumor_cell', 'Mast_cell', 'Regulatory_T_cell'], | Placeholder Source |
| PDAC             | 17, 7                          |['T_cells_Treg', 'T_cells_CD8+_effector_memory', 'T_cells_CD4-CD8-', 'B_cells_memory', 'B_cells', 'Monocytes_non-classical', 'Dendritic_cells', 'Monocytes_classical', 'T_cells_CD4+_naive', 'T_cells_CD4+_effector', 'T_cells_CD4+_effector_memory', 'NK_cells', 'Early_NK_cells', 'T_cells_CD8+_naive', 'T_cells_CD8+_effector', 'ILC', 'T_cells_CD4+_central_memory'], ['T_cells_CD4+', 'Dendritic_cells', 'T_cells_CD8+', 'T_cells_CD4-CD8-', 'B_cells', 'NK_cells', 'Monocytes'] | Placeholder Source |
| PBMC             | 7,8                              | ['T_NK', 'Endothelial', 'B_Plasma', 'Mast', 'Epithelial', 'Myeloid', 'CAFs'], ['Basal', 'CAFs', 'Myeloid', 'Mast', 'Classical', 'T_NK', 'Endothelial', 'B_Plasma'] | Placeholder Source |

## Using Statescope

The `Statescope` package allows you to choose different processed single-cell signatures. The package is located at the following repository:

[Statescope GitHub Repository](https://github.com/tgac-vumc/Statescope.git)

### Example Usage

```python
from Statescope import Initialize_Statescope

# Initialize the Statescope model with the desired parameters
Statescope_model = Initialize_Statescope(
    subset_bulk, 
    TumorType='NSCLC', 
    Ncelltypes='15', 
    Ncores=40
)
```

Replace the parameters as needed to specify the tumor type, number of cell types, and computational resources.
