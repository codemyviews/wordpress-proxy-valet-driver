# WordPress Proxy Valet Driver

> Proxy local `/uploads` requests to your production server. No more syncing uploads folders.

## Setup

1. Install the Valet Driver
	
	```bash
	wget https://raw.githubusercontent.com/codemyviews/wordpress-proxy-valet-driver/master/WordPressProxyValetDriver.php -O ~/.config/valet/Drivers/WordPressProxyValetDriver.php
	```
	
2. Enable the driver by adding a file called `.uploads-proxy` to your sites WP root, containing the URL that you wish to proxy to in `.uploads-proxy`. 

	In the one-liner below, **replace https://example.com with your actual production URL.** 

	```bash
	echo https://example.com >> .uploads-proxy	
	```
	
3. Done!
