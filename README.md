# 6D_pose_dataset
This repository contains Blender file that can be used for synthetic data generation for pose estimation in bin-picking scenarios.

## File format
The file contains a script Total.py. To add a custom mesh model, change the following line,
<pre><code>mesh = filename
</code></pre>
to include the name of your mesh <code>mesh_name.ply</code>. The number of objects in the container <code>N</code> is set to 20, the size of the bin is <code>pos=15</code>. The total number of rendered scenes is given by, <code><i>lm</i> x <i>num_sample</i></code>, which is the product of the number of unique bin-picking arrangements and the number of in-plane rotations given to the camera.
## Dependencies
Blender 2.79.

## License
This repository is released under the . Refer to LICENCE for more details. 
