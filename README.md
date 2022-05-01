## Environment Setup for Nintendo Switch
Project involves coding with Ubuntu L4T framework with nintendo switch


### Setup the environment to force exporting 1080p 

	echo "1920x1080" | sudo tee /etc/dock-hotplug.conf

### To run the docker support ROS packages:

	sudo docker run -it nvidiajetson/deepstream-ros2-foxy:5.0.1
	
### Setup proxy environment 

Install v2ray latest release

	bash <(curl -L https://raw.githubusercontent.com/v2fly/fhs-install-v2ray/master/install-release.sh)

Then install proxychains4 

	sudo apt install proxychains4
	
Update the proxychains4 default configuration

	sudo gedit /etc/proxychains4.conf
	
Now you can run any command using proxychains4 

	proxychains4 curl myip.ipip.net



## Useful Links

#### How to install swtichroot L4T Ubuntu Bionic (18.04): 

https://wiki.switchroot.org/en/Linux/Ubuntu-Install-Guide

#### About The Robot Operating System (ROS)

https://docs.ros.org/en/foxy/index.html
