1. Create a workspace similar to how you create catkin workspaces with an empty src folder inside 

2. rosinstall_generator image_transport_plugins --rosdistro kinetic --deps --wet-only --tar > NAME.rosinstall

3. wstool init -j8 src <NAME.rosinstall>

4. catkin config --install --install-space /opt/ros/kinetic/ -DCMAKE_BUILD_TYPE=Release

5. catkin build
