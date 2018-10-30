FROM ubuntu:latest

#RUN apt-get install tshark
RUN apt-get install -y netcat
RUN apt-get update && apt-get install -y tcpdump && sleep 5

#RUN nohup nc -vlkp 8080 
#RUN tcpdump -i eth0 not udp -vv 
#RUN tshark -i eth0 -w capture-output.pcap

RUN tcpdump -i eth0 not udp -vv 

#RUN ( tcpdump -n -i eth0 not udp port 53 and ip -c 1 -t | sed -e 's/^[^$]/internet traffic: /' ) 
