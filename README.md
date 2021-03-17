# [PLS-VIO] Comparison of 4-parameter orthogonal expression and 2-parameter expression proposed by our paper of line features.
This repository is supplementary material that provides the simulation code for running and comparison results. After we generate the simulated straight line observations, we initialize them to obtain the straight line in the three-dimensional space and optimize the  line landmarks. The code is the initial version, and it will be improved further in the comming months.
<center class="half">
    <img src=./bin/demo/simulate_line.gif width="300"/><img src=./bin/demo/simulate_line.png width="300"/>
</center>

## 1. Prerequisites
1.1 **Ubuntu** and **ROS**

Ubuntu 16.04, python3.

1.2. **Dependency**

Eigen 3.3.1, OpenCV 3.3.9, Cere-solver 2.0.0: [Ceres Installation](http://ceres-solver.org/installation.html), remember to **sudo make install**.

## 2. Build Project with Cmake
Clone the repository and compile the project:
```

	git clone https://github.com/xubogithub/Structural-and-Non-structural-line.git
	cd ~/Structural-and-Non-structural-line-master/
	mkdir build
	cd build
	cmake ..
	make -j4   
```
**Notice**: The executable file **line_optimization** is in the bin directory, and you can run it by **./line_optimize**

## 3. Python Tools for Visualization
We provide some visualizaton tools for comparison and analysis.
Visual simulation animation:
```
	python draw_points.py
```
Visual simulation trajectory and line landmarks:
```
	python plot_simulate.py
```
Visual results of the code:
```
	python plot_result.py
```
## 4. Related Papers

- **Leveraging Structural Information to Improve Point Line Visual-Inertial Odometry**.
```
The paper is received.
```

We use [vio_data_simulation ](https://github.com/HeYijia/vio_data_simulation.git) as our base line code and generate the simulation data.

## 5. Acknowledgements

Thank Dr. Yijia He very much. We are still working on improving the code reliability. For any technical issues, please contact Bo Xu boxu1995@whu.edu.cn and Peng Wang cypminxuan@163.com.

## 6. Licence
The source code is released under [GPLv3](http://www.gnu.org/licenses/) license.
