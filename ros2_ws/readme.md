### Connection and collecting data:

## Running VLP-16 ros2 driver
VLP-16 IP: 192.168.2.201
- Connect to jetson using ssh (username: nvidia, password: nvidia) , it is configured to connect to the following wireless netowork (SSID: B3, Password: qwert123) this can be changed manually.
```bash
source /opt/ros/foxy/setup.bash
source /media/nvidia/ssd/home/nvidia/ros2f/install/setup.bash
sudo ifconfig eth0 down
sudo ifconfig eth0 192.168.2.102 netmask 255.255.255.0
ros2 launch velodyne velodyne-all-nodes-VLP16-launch.py
```
