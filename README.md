# Point-Cloud-Test

Point clouds of different resolution for latency testing. This repository uses the [FR-079 corridor](http://ais.informatik.uni-freiburg.de/projects/datasets/octomap/) octree sample.

The original octree was converted to .pcd format using octomap, then converted to .ply format using pcl.

    ./octree2pointcloud fr_079.bt pcl/d.pcd
    ./pcl_pcd2ply 1 1 trees/d.pcd ply/d.ply
