# ethercat_driver_ros2
[![Licence](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![DOI](https://zenodo.org/badge/491930126.svg)](https://zenodo.org/badge/latestdoi/491930126)
[![Build](https://github.com/ICube-Robotics/ethercat_driver_ros2/actions/workflows/ci.yml/badge.svg)](https://github.com/ICube-Robotics/ethercat_driver_ros2/actions/workflows/ci.yml)

Implementation of a `Hardware Interface` for simple Ethercat module integration with [`ros2_control`](https://github.com/ros-controls/ros2_control) and building upon [IgH EtherCAT Master for Linux](https://etherlab.org/en/ethercat/).

## About
[EtherCAT](https://www.ethercat.org/default.htm) provides applications with the capacity of reliable, real-time communication between systems and is therefore a common industrial standard. In order to simplify the development/deployment of new application using EtherCAT modules, the `ethercat_driver` allows to combine them with [`ros2_control`](https://github.com/ros-controls/ros2_control). This driver proposes a generic ways to parametrise and assemble `Hardware Interfaces` based on EtherCAT modules that can be defined using parameter files.

**For more information, please check the [documentation](https://ICube-Robotics.github.io/ethercat_driver_ros2/).**

# Build
Clone this repo as a package inside a ros2 workspace, like `git clone this_repo_url ~/ros2_ws/src`.
Using the below command to build the entire workspace and choose the etherlab location as you would like to:
```sh
colcon build --symlink-install --cmake-args ' -DCMAKE_BUILD_TYPE=Release' ' -DETHERLAB_DIR=/opt/etherlab'
```

## Acknowledgments
Parts of the driver are based on the implementation of [`SimplECAT`](https://bitbucket.org/bsoe/simplecat/src/master/).

## Contacts ##
![icube](https://icube.unistra.fr/fileadmin/templates/DUN/icube/images/logo.png)

[ICube Laboratory](https://icube.unistra.fr), [University of Strasbourg](https://www.unistra.fr/), France

__Manuel Yguel:__ [yguel@unistra.fr](mailto:yguel@unistra.fr)

__Laurent Barbé:__ [laurent.barbe@unistra.fr](mailto:laurent.barbe@unistra.fr)

__Philippe Zanne:__ [philippe.zanne@unistra.fr](mailto:philippe.zanne@unistra.fr)

__Maciej Bednarczyk:__ [m.bednarczyk@unistra.fr](mailto:m.bednarczyk@unistra.fr), @github: [mcbed](https://github.com/mcbed)
