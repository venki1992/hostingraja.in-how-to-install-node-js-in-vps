# hostingraja.in-how-to-install-node-js-in-vps
The following steps are to be followed to install node js on the VPS server


Installation Method:

echo -e "--------------------------------"

echo -e "1.Node.js v6"

echo -e "2.Node.js 8"

echo -e "--------------------------------"

echo -e "Enter your option >"

read javaversion

case "$javaversion" in

1)

curl --silent --location https://github.com/nodesource/distributions/blob/master/rpm/setup_6.x | sudo bash -
;;

2)
curl --silent --location https://github.com/nodesource/distributions/blob/master/rpm/setup_8.x | sudo bash -
    ;;
    
*) echo -e "You have entered wrong option. Try aftesometime"
   ;;
esac

yum -y install nodejs git  gcc-c++ make

npm install -g pm2

npm install -g grunt-cli

npm install -g gulp

npm install webpack -g


the above user interaction script gets the version which will need to install. Currently, HostingRaja provides the stable release of Node.js version 8.9.3 ( Recommended by most of the user )  and we have given the earliest version of Node.js6 also.  

Node Js:

Node.js is an open-source, cross-platform JavaScript run-time environment for executing server-side JavaScript code. Mostly, we have used JavaScript for client-side scripting,  Node.js enables JavaScript to be used for server-side scripting, and runs scripts server-side to produce dynamic web page content before the page is sent to the user's web browser. Finally, Node.js has become one of the foundational elements of the "JavaScript everywhere" paradigm. 

Why we will use Node.Js:

1. CPU High usage: 
If your RTA( Real Time Application ) has taken more memory usage then we will choose the Node.js  because Node.js is based on an event-driven, non-blocking I/O model, and uses only a single CPU core. 
2. Better browsers and faster javaScript engine
3. It makes your application as more scalable 
4. Package Availability: Many packages for Node.js applications are available in npm . npm is the largest available repository at the moment that has helpful to built the application within a short time span 

Like node.js HostingRaja supports lots of coding peripherals. Visit hostingraja.in to know more

