V-REP ROS plugin
========

Vrep ROS plugin with customized commands.
Used for KUKA challenge. 

Original sources and binaries can be found at http://www.coppeliarobotics.com


### Dependencies

* ROS (i use fuerte)
* V-REP

### Building instruction

* Put this folder into your ROS workspace
* `cd vrep_common`
* `mkdir build && cd build && cmake .. && make -j`
* `cd vrep_plugin`
* Remove my symbolic links and create yours, pointing to the right V-REP folders (/programming/include and /programming/common).
* `mkdir build`
* `cd build && cmake .. && make -j`
* Modify build.sh to reflect your folder hierarchy, it should copy the newly generated /lib/libv_repExtRos.so into your V-REP main folder

### License
V-REP is published under GNU GPL.

For further information, check out [this page](http://www.coppeliarobotics.com/licensing.html).
