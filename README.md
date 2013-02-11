# Nodeployer

Use nodeployer for GitHub continous deployment to Amazon EC2. It is a superior alternative to capistrano. 

## Usage

SSH into your Amazon EC2 instance and run the following.

    $ sudo apt-get install nodejs npm
    $ mkdir repos
    $ cd repos
    $ git clone git@github.com:scottmotte/nodeployer.git
    $ cd nodeployer
    $ npm install
    $ node app.js