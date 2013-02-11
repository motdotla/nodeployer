# Nodeployer

Use nodeployer for GitHub continous deployment to Amazon EC2. It is a superior alternative to capistrano. 

## Usage

SSH into your Amazon EC2 instance and run the following.

    $ cd .ssh
    $ ssh-keygen -t rsa -C "your_email@youremail.com"
    $ cat id_rsa.pub (copy the key and add it to your keys in your github settings)
    $ sudo apt-get install nodejs npm
    $ mkdir repos
    $ cd repos
    $ git clone git@github.com:YOURNAME/REPO_NAME.git
    $ git clone git@github.com:scottmotte/nodeployer.git
    $ cd nodeployer
    $ npm install
    $ REPO_NAME=name_of_your_repo node app.js
    $ visit yourec2instance.amazon.com:3000

Make sure port 3000 is opened up on your EC2 instance.