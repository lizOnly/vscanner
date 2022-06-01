# vscanner

It is a virtual scanner that takes a mesh  in ply format as input, and outputs a ptx pointcloud with its respective panoramic image

## Dependencies

[gproshan]: https://github.com/larc/gproshan/tree/alpha

 

Install all dependencies and run:

	mkdir build
	cd build
	cmake ..
	make

finally execute:

	./scanner [mesh_paths.(ply)]  ncols_image nrows_image 0.01 [pointcloud_output_path]

### 

