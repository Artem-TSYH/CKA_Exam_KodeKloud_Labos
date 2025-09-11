Linux-Commands:
- ip 
-- ip a 
-- ip a show type bridge 
-- ip route 

- ss
- netstat (old version of "ss"-command) 
-- ss -nlp
-- ss -ntp | grep etcd

# 7/12. . . . 

ip a show help
ip a show type bridge
ip address show type bridge

# 9/12. If you were to ping google from the controlplane node, which route does it take? What is the IP address of the Default Gateway?

ip route

# 11/12. Notice that ETCD is listening on two ports. Which of these have more client connections established?

ss -ntp | grep etcd
ss -npa | grep etcd (alternative)