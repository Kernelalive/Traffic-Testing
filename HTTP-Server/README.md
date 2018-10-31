# Http Server-Node js 
A Simple HTTP  Node js server running on Docker container Only for Testing 
To run it properly simpl run	
```
	1. Build the image (docker build -t http-server-js .)
	2. Run the docker with the image created on step 1 exposing the ports that envoy listens to (8080)(docker run --rm -it -p 8080:8080 --name http-server-js http-server-js:latest)
	3. Test if everything works. (127.0.0.1:8080)
```
