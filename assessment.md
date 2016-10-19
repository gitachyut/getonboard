##1. Restart apache/nginx webserver from a webpage.<br>

-> As apache/nginx restart process runs via sudo command.
So need to edit /etc/sudoers file and add lines similar to the following;<br>

```Cmnd_Alias      RESTART_APACHE = service httpd restart```<br>
```www-data ALL=NOPASSWD: RESTART_APACHE```<br>

Now we don't need to add sudo before the command in the script which will be run through a webpage.<br>
In php code:- ```<?php exec('service httpd restart'); ?>```<br>

##2.Use Facebook API to post status update, write a program to fully Implement the solution<br>

-> https://github.com/gitachyut/fb_status_update

##3. Prepare a CLI client that will Login to Facebook and post a status update.<br>

-> https://github.com/gitachyut/fb_cli_app

##4. Write a program that will download that flipkart URL and then parse with regex to get the product name, big images and breadcrumb. https://www.flipkart.com/apple-iphone-6s-plus/p/itmebysggwdsvyytm?pid=MOBEBY3VR4DUEPUJ<br>

-> As flipkart is a progressive (app shell architecture) and recat.js based  webapp, so it just render the app shell (mainly the UI part and SEO tags) in server side rendering and then in client side, it run the scripts to load the DB contents using ajax calls, all these happens the browser environment. So using some program I can surly download the URL but most of the div e.g. like ```<h1 class="_3eAQiD"><!-- react-text: 1815 -->Apple iPhone 6S Plus (Gold, 16 GB)<!-- /react-text --></h1>```, images tag ```<img class="sfescn" src="https://rukminim1.flixcart.com/image/832/832/mobile/b/u/7/apple-iphone-6s-plus-mku82hn-a-original-imaehudwsdrtmhhe.jpeg?q=70">``` will not be available in the downloaded file and as a result wouldn't be able to parse the required elements.

So my main point is, I really don't know how to scrap this type of webapps. That's why I want to work
with your team :smiley: but I do know regex

##5. Fix Internal Server Error​ at http://ec2-54-254-158-171.ap-southeast-1.compute.amazonaws.com/<br>

-> Fixed.
