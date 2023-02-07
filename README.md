# Practice Package
Create a ROS 2 package, build it and use it. 

## Instructions: 
1. (30%) Create a ROS package with a Python executable script use command: `ros2 pkg create --build-type ament-python --node-name <executable_name> <node_name>`. **Reference: [Creating a package](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Creating-Your-First-ROS2-Package.html)**
2. (40%) Modify the executable python file to publish `String()` message under the topic `/robot/hello_world` with content "Hello World". The topic should be published with the frequency of 10 Hz. **Reference: [Writing a simple publisher and subscriber (Python)](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Writing-A-Simple-Py-Publisher-And-Subscriber.html)**
3. (20%) Use `colcon build` to make your package and the executable python script usable (executable using `ros2 run <your_package_name> <executable_name>`). **Reference: [Creating a package](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Creating-Your-First-ROS2-Package.html)**
4. (10%) Edit `package.xml` and `setup.py` in your package directory. Fill `<maintainer>`, `<maintainer_email>`, `<description>` or any other fields with appropriate information. **Reference: [Creating a package](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Creating-Your-First-ROS2-Package.html)**

#### Hint:
Don't forget to source the overlay (your package) by `source ~/<ros_workspace_name>/install/local_setup.bash`. Or you (**only need to do this once**) can automatic source it by adding the command to `~/.bashrc` by `echo "source ~/<ros_workspace_name>/install/local_setup.bash" >> ~/.bashrc`. You'll replace <ros_package_name> to your actual ROS workspace name.
