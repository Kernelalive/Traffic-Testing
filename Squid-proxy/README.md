# Squid Proxy
A Squid  inside a docker container
To run it properly :

	
```	
	0. Navigate to the right directory.
	1. Build the image (docker build  -t tha-squid .)
	2. Run the docker with the image created on step 1 (docker run --name squid-proxy -d --restart=always   --publish 3128:3128   --volume /srv/docker/squid/cache:/var/spool/squid tha-squid:latest)
	3. Attach to the container you have just created (docker exec -it squid-proxy bash). And check the access log to see if the requests for the host are going through squid proxy (tail -f /var/log/squid/access.log)
	4. Open a new terminal and set the ENVs for forwarding every request to the docker bridge and to the port that squid listens to.  (export http_proxy=http://172.17.0.1:3128, export https_proxy=http://172.17.0.1:3128, ftp_proxy=http://172.17.0.1:3128 )
	5. curl -v http://google.com for one terminal and check to the other terminal if the request is being forwarded in the squid proxy docker.
```

More to come !! :+1
