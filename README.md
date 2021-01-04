## RoboND - Build My World

---

### World Layout

![Top view](/image/world2_top.jpg)

![Perspective view](/image/world2_perspective.jpg)

### Robot Layout

![Top view](/image/robot_transparent.jpg)

![Top view](/image/robot_wireframe.jpg)

### Dependencies

- ROS Kinetic
- CMake 2.8

### Build Instruction

1. Build the plugin `welcome_message.cpp`.

    ``` shell
    $ mkdir build && cd build
    $ cmake ..
    $ make
    ```

2. Export the `build` directory path to `GAZEBO_PLUGIN_PATH` environment variable, so that the built plugin libraries can be loaded by Gazebo

    ``` shell
    $ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:${PWD}
    ```

3. Load the `Library` world from Gazebo

    ``` shell
    $ cd ../world
    $ gazebo Library.world
    ```