- ## Documentation of Lordchancellor's Project 4
- Summary: In this project, i got familiar with the MEAN web stacks(MongoDB, Express, Angular and Node.js) amd deployed it to the ubuntu server through the AWS cloud. Check the image below to see the successful connection to ubuntu server on AWS cloud
![Ubuntu server on AWS cloud](https://github.com/Lordchancellorr/project-4/blob/main/Images/Successful%20connection%20to%20Ubuntu%20server%20in%20AWs%20cloud.PNG)
= ## Implementation of Instructions in Step 1
- The first ideal commands ran on the ubuntu server was `sudo apt update` and `sudo apt upgrade` to ensure i was using the latest version of ubuntu. Check the image below for the output. 
![Sudo apt update](https://github.com/Lordchancellorr/project-4/blob/main/Images/Sudo%20apt%20update.PNG)
- For certification purpose, i ran `sudo apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates` alongside `curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -` on the ubuntu server.
- I started with the installation of Nodejs as instructed in the documentation. Then i ran the following commands- `sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6` and `echo "deb [ arch=amd64 ] https://repo.mongodb.org/apt/ubuntu trusty/mongodb-org/3.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.4.list`
- I installed mongodb with this command- `sudo apt install -y mongodb` and the image below was the status of mongodb after i ran `sudo systemctl status mongodb`
![status of mongodb](https://github.com/Lordchancellorr/project-4/blob/main/Images/Status%20of%20mongodb.PNG)
- I ran `sudo apt install -y npm` to install the node package manager and `sudo npm install body-parser` to install the body parser. check the image below
![body parser](https://github.com/Lordchancellorr/project-4/blob/main/Images/body%20parser%20installation.PNG)
 As stated in the documentation, i created a directory named as books with this command `mkdir Books && cd Books` and initialized the npm project with the command `npm init` I created a file and named it server.js inside the books directory and pasted the codes inside the documentation with the command `vi server.js`
- ## Implementation of Step 2-4
- I ran `sudo npm install express mongoose` to install express and mongoose at the same time and the image below was the output:
![status of express and mongoose](https://github.com/Lordchancellorr/project-4/blob/main/Images/express%20and%20mongoose%20installation.PNG)
i created another directory with this command `mkdir apps && cd apps` and created a file inside the apps directory with the command `vi routes.js` pasted and saved the codes inside the documentation inside the file. In the apps directory, i create another foler with this command `mkdir models && cd models` and created a file inside the models directory with the code `vi book.js` (some codes were pasted here)
= With `cd ../..` i returned to the Boos directory and created another directory with this command `mkdir public && cd public` inside which 
- I created anew file with `vi script.js` and pasted the codes inside the documentation and saved it accordingly. Inside the public directory, i created a new file with `vi index.html` and pasted soem codes inside. In the Books directory, i ran `node server.js` and the image below was the output
![node server.js](https://github.com/Lordchancellorr/project-4/blob/main/Images/node%20server.js)
- I accessed the Book register web application after changing my security inbound rule to TCP, Port 3300. With my IP address and:3300, the image below was the result:
![completion of project 4](https://github.com/Lordchancellorr/project-4/blob/main/Images/Completion%20of%20project%204.PNG). I edited the appliaction to test if it is functioning properly and it did. Check the image below for the result. 
![test run](https://github.com/Lordchancellorr/project-4/blob/main/Images/Test%20run.PNG)

This brings us to the completion of successful implementation of project 4. Thanks for your patience!