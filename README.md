# 6D pose dataset
This repository contains Blender file that can be used for synthetic data generation for pose estimation in bin-picking scenarios.

## Using the .blend file
To use the file, open Blender and load the Blender file. First run the mat.py script to generate a custom Material. To change the material properties, vary the node properties.

### To generate the dataset
The file contains the script Total.py that generates bin-picking dataset for the custom brick model. The script Total_mesh.py generates dataset for the [T-LESS](http://cmp.felk.cvut.cz/t-less/) mesh model. To add a custom mesh model, change the following line in this script,
<pre><code>mesh = bpy.ops.import_mesh.ply(filepath="/home/nuclides/Documents/MTech Project/blender/red bricks/mesh.ply")
</code></pre>
to include the name of your mesh <code>mesh_name.ply</code>. The number of objects in the container <code>N</code> is set to 20, the size of the bin is set as <code>pos=15</code>. The total number of rendered scenes is given by, <code><i>lm</i> x <i>num_sample</i></code>, which is the product of the number of unique bin-picking arrangements and the number of in-plane rotations given to the camera. Also, change the <code>filepath</code> to the desired destination.
The mesh models can be found in <code>models</code>.

## Dependencies
Blender 2.79.

## License
This repository is released under the GNU General Public License v3.0. Refer to LICENCE for more details. 
