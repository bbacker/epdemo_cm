Entertainment Partners - Platform Engineering Test
======================


## Challenge

Entertainment Partners is a rapidly-changing environment that requires our engineers to think of infrastructure as code. Please demonstrate your ability to hit the ground running when it comes to SDLC practices, project design, and configuration management principles. We understand that many tools serve the CM space. Please choose *one* of your favorite configuration management tools. Using that tool, spend no more than 90-120 minutes configuring the webserver to yield a working web page at http://localhost:8080 with a single invocation of `vagrant up`. Your deliverable is to email back the Vagrantfile that will allow this. Submissions that do not meet this requirement will not be considered.

   * Using the supplied Vagrantfile, modify it as you wish but the leave vm.box as is
   * Install and configure PHP-FPM
   * Install and configure NGINX to proxy web requests to PHP-FPM
   * Deploy the supplied app.php to web root
   * Services must survive a reboot (`vagrant reload`)
        *No shell commands or their equivalent, use tool built-ins only
