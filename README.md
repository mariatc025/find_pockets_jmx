# Find Pockets Algorithm
Repository for the SBI/Python project.
<p align="center">
  <img src="https://github.com/user-attachments/assets/cb99cf45-d5ed-4b92-85ec-7d17d032e7c1" width="600">
</p>

## Description
Ligand-binding site prediction tool based on a geometric approach. For a more detailed description of the algorithm, usage and output of the program check the report.

## Usage
``
python find_pockets.py path/to/pdb_file.pdb
``

## Advanced Options
Although not recommended you can adjust parameters shuch as the voxel size, probe radius and MIN_PSP if needed in the run_complete_workflow() function, for instance:

```python
run_complete_workflow(
file_path="1a6u.pdb",
output_dir="./output"
voxel_size=0.4, # Higher resolution (slower)
MIN_PSP=2, # Lower threshold for noisy data
probe_radius=1.2 # Smaller solvent probe
) ```
