# Point-Cloud-Test

Point clouds of different resolution for latency testing. This repository uses the [FR-079 corridor](http://ais.informatik.uni-freiburg.de/projects/datasets/octomap/) octree sample.

To use the `octree2pointcloud` binary, compile the [Octomap](https://github.com/OctoMap/octomap) library. The binary is located in the `octomap/bin`.

To use the `pcl_pcd2ply` binary, compile the [Point Cloud Library](https://github.com/PointCloudLibrary/pcl). The binary is located in either `pcl/build/bin` or `pcl/bin`, depends on how you set up the build directories.

The original octree was converted to .pcd format using octomap, then converted to .ply format using pcl.

    ./octree2pointcloud fr_079.bt pcl/d.pcd
    ./pcl_pcd2ply 1 1 trees/d.pcd ply/d.ply
