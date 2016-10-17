1. Restart apache/nginx webserver from a webpage.
-> As apache/nginx runs under access to restart Apache via the sudo command.
So need to edit /etc/sudoers file and add lines similar to the following:

Cmnd_Alias      RESTART_APACHE = service httpd restart
www-data ALL=NOPASSWD: RESTART_APACHE

so that we don't need to add sudo before the command in the script which will be run through a webpage
in php <?php exec('service httpd restart'); ?>

2.Use Facebook API to post status update

-> https://graph.facebook.com/user_id/feed?message=Helloworld!&method=post&access_token=your_fb_open_graph_app_token


3. Prepare a CLI client that will Login to Facebook and post a status update.
->

4. Use regex to parse product name, big images and breadcrumb for
https://www.flipkart.com/apple-iphone-6s-plus/p/itmebysggwdsvyytm?pid=MOBEBY3VR4DU
EPUJ

5. Fix Internal Server Error​ at
http://ec2-52-221-252-33.ap-southeast-1.compute.amazonaws.com/
Use the private key to SSH into the server with username ec2-user

-> fixed, .htaccess file had some issue.
