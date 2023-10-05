# Branch `[kirkstone]`

As of Milestone 17 (2022-06-05), this branch can be used to build the releases
current in mid-November 2021 of ROS 2 **foxy** and **galactic** and **humble** and ROS 1
**melodic** and **noetic** with the **kirkstone** OpenEmbedded release series as
of the beginning of December 2021.

The mid-November 2021 release (and earlier releases) of ROS 2 **rolling** can no
longer be built because the commits referenced by its recipes have been removed
from the `[release/rolling/*]`branches of the release repositories.

A "best effort" has been made to keep the EOL-ed ROS 2 **dashing** and
**eloquent** distros buildable, but some of the packages that are used to create
the `ros-image-world` image do not build. However, the `ros-image-core` image
does successfully build.

Instructions for using `meta-ros` are
[here](https://github.com/ros/meta-ros/wiki/OpenEmbedded-Build-Instructions).

## Status

With the exception of the commits added to complete Milestone 17, this repository
has not been maintained since December 2021. Its future maintenance was
discussed in the
[OSRF TSC January 2022 meeting post](https://discourse.ros.org/t/os-2-tsc-meeting-january-20th-2022/23986/2).

## History

The original implementation of `meta-ros` for ROS 1 Indigo Igloo
(<https://github.com/bmwcarit/meta-ros>) was transferred here on 2019-06-25. It
has been converted to use recipes generated by
[superflore](https://github.com/ros-infrastructure/superflore/). Please see this
[wiki page](https://github.com/ros/meta-ros/wiki/Superflore-OE-Recipe-Generation-Scheme)
for details of what was done and the current development milestones.

The original implementation has been retained in the
[`legacy`](https://github.com/ros/meta-ros/tree/legacy) branch.
