# ROS2-Service-Activities

Activity 003 - ROS2 Services
Let’s practice with ROS2 Services!

You will start from the Topic activity you did in the last section on Topics.

Here is what you got:

![image](https://github.com/promit7473/ROS2-Service-Activities/assets/108547743/04a048bb-c78a-496b-bf19-2c081a8d38e7)



Quick recap:

The node “number_publisher” publishes a number on the /”number” topic.

The node “number_counter” gets the number, adds it to a counter, and publishes the counter on the “/number_count” topic.

And now, here is what you’ll add:

![image](https://github.com/promit7473/ROS2-Service-Activities/assets/108547743/8b9eb81f-b6a2-4351-b72b-09d188c98334)



Add a functionality to reset the counter to zero:

Create a service server inside the “number_counter” node.

Service name: “/reset_counter”

Service type: example_interfaces/srv/SetBool. Use “ros2 interface show” to discover what’s inside!

When the server is called, you check the boolean data from the request. If true, you set the counter variable to 0.

We will then call the service directly from the command line. You can also decide - for more practice - to create your own custom node to call this “/reset_counter” service.

And of course, as always, you can do the activity for both the Python and Cpp versions.

