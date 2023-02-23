# Practice Package
Create a ROS 2 package, build it and use it. 

## Instructions: 
1. (30%) Create a ROS package with a Python executable script use command: `ros2 pkg create --build-type ament_python --node-name <executable_name> <package_name>`. **Reference: [Creating a package](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Creating-Your-First-ROS2-Package.html)**
2. (40%) Modify the executable python file to publish `String()` message under the topic `/robot/hello_world` with content "Hello World". The topic should be published with the frequency of 10 Hz. **Reference: [Writing a simple publisher and subscriber (Python)](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Writing-A-Simple-Py-Publisher-And-Subscriber.html)**
3. (20%) Use `colcon build` to make your package and the executable python script usable (executable using `ros2 run <your_package_name> <executable_name>`). **Reference: [Creating a package](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Creating-Your-First-ROS2-Package.html)**
4. (10%) Edit `package.xml` and `setup.py` in your package directory. Fill `<maintainer>`, `<maintainer_email>`, `<description>` or any other fields with appropriate information. **Reference: [Creating a package](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Creating-Your-First-ROS2-Package.html)**

#### Hint:
Before verify step 3, don't forget to source the overlay (your package) by `source ~/<ros_workspace_name>/install/local_setup.bash`. Or you can automatically source it whenever you open a new terminal by adding the command to `~/.bashrc` (**only need to do this once**). `echo "source ~/<ros_workspace_name>/install/local_setup.bash" >> ~/.bashrc` will get the job done. You'll replace <ros_workspace_name> with your actual ROS workspace name.
