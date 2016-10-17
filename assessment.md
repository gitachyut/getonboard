##1. Restart apache/nginx webserver from a webpage.<br>

-> As apache/nginx restart process runs via sudo command.
So need to edit /etc/sudoers file and add lines similar to the following:<br>

```Cmnd_Alias      RESTART_APACHE = service httpd restart```<br>
```www-data ALL=NOPASSWD: RESTART_APACHE```<br>

So that we don't need to add sudo before the command in the script which will be run through a webpage.<br>
In php code:- ```<?php exec('service httpd restart'); ?>```<br>

##2.Use Facebook API to post status update<br>

-> https://graph.facebook.com/user_id/feed?message=Helloworld!&method=post&access_token=your_fb_open_graph_app_token


##3. Prepare a CLI client that will Login to Facebook and post a status update.<br>
-> We can use ```"fbcmd"``` package

##4. Use regex to parse product name, big images and breadcrumb for
https://www.flipkart.com/apple-iphone-6s-plus/p/itmebysggwdsvyytm?pid=MOBEBY3VR4DUEPUJ




##5. Fix Internal Server Error​ at
http://ec2-52-221-252-33.ap-southeast-1.compute.amazonaws.com/<br>
Use the private key to SSH into the server with username ec2-user

-> fixed, ```.htaccess``` file had some issue.
