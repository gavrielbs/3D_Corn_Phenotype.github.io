# 3D_Corn_Phenotype

## Point Cloud Files

All point cloud files are stored under `samples/round_2/<scanned date>/<plant number>`.

### Point Cloud Files Naming Convention

- `<scanned date>_<plant number>.xyz` - `28.2.23_1.xyz`  

  Unprocessed point cloud, containing pot and background.  

  TSV file consisting of columns: x, y, z, r, g, b

- `<scanned date>_<plant number>_edited.txt` - `28.2.23_1_edited.txt`  
  Processed point cloud, containing only maize plant.  
  TSV file consisting of columns: x, y, z, r, g, b

- `<scanned date>_<plant number>_edited_no_rgb.txt` - `28.2.23_1_edited_no_rgb.txt`  
  Processed point cloud, containing only maize plant.  
  TSV file consisting of columns: x, y, z

- `<scanned date>_<plant number>_edited_no_rgb_labeled.txt` - `28.2.23_1_edited_no_rgb_labeled.txt`  
  Processed point cloud, containing only maize plant.  
  Output of Label3DMaize, each organ (leaf/stem) labeled separately.  
  TSV file consisting of columns: x, y, z, label

- `<scanned date>_<plant number>_constructed.txt` - `28.2.23_1_constructed.txt`  
  Processed point cloud, containing only maize plant.  
  Initial output of CNN model, downsampled point cloud.  
  Labels: stem = 1, leaf = 0  
  TSV file consisting of columns: x, y, z, label

- `<scanned date>_<plant number>_constructed_refined_radius_<radius>.xyz` - `28.2.23_1_constructed_refined_radius_0.01.txt`  
  Processed point cloud, containing only maize plant.  
  Final output of CNN model, original point cloud.  
  Labels: stem = 1, leaf = 0  
  TSV file consisting of columns: x, y, z, label
