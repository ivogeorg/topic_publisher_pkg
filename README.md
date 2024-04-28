### topic_publisher_pkg

`roslaunch topic_publisher_pkg topic_publisher_launch_file.launch`

### Notes

1. This package was created _after_ another one, called [`my_package`](https://github.com/ivogeorg/my_package) in the same `~/catkin_ws/src` tree. `catkin_make` didn't find the new package, even though `roscd topic_publisher_pkg` worked found, inlucing the command-line completion. Based on [this](https://answers.ros.org/question/215173/catkin_make-does-not-compile-all-packages-in-the-workspace/) discussion, the solution was to delete the `build` and `devel` directories and rerun `catkin_make`. This time it found and built both packages.
