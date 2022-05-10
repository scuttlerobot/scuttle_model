# scuttle_model

Provides a user customizable wrapper for `scuttle_desciption` that allows you to add your own
components to SCUTTLE.

## Dependencies

The configurations in this repository assume you have the following prerequisites installed on the
device on which you want to run this code. That device might be an Ubuntu machine or a physical
SCUTTLE using Raspberry Pi OS.

1. [ROS Noetic](http://wiki.ros.org/noetic) with the `ros-noetic-navigation`, `ros-noetic-robot` and
   `ros-noetic-tf2` packages.
1. A working [ROS workspace](http://wiki.ros.org/catkin/Tutorials/create_a_workspace).
1. The [scuttle_description](https://github.com/scuttlerobot/scuttle_description) package installed
   in your workspace.

## Usage

To use the `scuttle_model` package you need to take the following steps

1. Clone this repo into the `src` directory of your ROS workspace
1. Create a new URDF file in the `urdf` directory. Add your own components to this new URDF file.
1. Add a link to your URDF file in the `urdf/scuttle.xacro` file.
1. Build your workspace using `catkin_make`

Once you have taken these steps you can run your model in Gazebo, for instance using one of the
worlds defined in the [scuttle_gazebo](https://github.com/scuttlerobot/scuttle_gazebo) repository.
