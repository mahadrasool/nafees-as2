Automation With ansible.

Here i am implementing a simple web service by using nginx.

The basic service is an Nginx web server, that can only serves one simple page. That page renders the hostname, IP and the port of the server running it.

We need to run multiple web servers on three different platforms. So, HAproxy is used to load balance between these three services. The site has 5 hosts HAproxy, A, B, C and Bastion. 

HAproxy runs as an entry point for accessing the service from the servers. Bastion acts as an SSH entry point to the internal network.

Create an SSH-keygen and use the public key in the servers. 

The SSH file has to be modified in terms of your ip addresses of your servers and the ssh private key path.
