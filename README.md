# robot_gui_bridge
This is a ROS1 package to setup a web GUI to control a robot and stream a video feed.

## Usage
- Install the [`http-server`](https://www.npmjs.com/package/http-server) package.
- Use `roslaunch robot_gui_bridge websocket.launch` to start the rosbridge_websocket 
- Change to the gui directory and start the web gui with `http-server`
- http-server will give you an ip-address to access the web gui

`sensor_msgs/Joy` will be published on the `/joy` topic.

To get the video streamed you would additionally need to launch the [web_video_server](http://wiki.ros.org/web_video_server)
