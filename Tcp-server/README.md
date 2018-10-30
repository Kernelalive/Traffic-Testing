# Tcp Server
A Simple TCP server running on Docker container Only for Testing 
To run it properly simpl run	
```
	1. Build the image (docker build -t tcp_server .)
	2. Run the docker with the image created on step 1 exposing the ports that netcat listens to (8080)(docker run --rm -it -p 8080:80 --name tcp_server tcp_server:latest)
	3. Use traffic generator to test it.)
```
