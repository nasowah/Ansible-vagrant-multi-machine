# Ansible + vagrant multi-machine
This is learning project to set up an infrastructure running:

1 load balancer,
2 Application / Web Servers
2 Database Servers

## Intention of the project
The intent is to mimic the provissioning and management of a production server for practive.

So why 5 guest machines? Okay, this is what I want to do:

- Set up 2 servers to run applications / web at the same time. More like a production system.
- Set up 2 DB servers. Run 1 as primary OLTP and run the other as reporting with replication between them.
- Set up a load balancer to share the traffic between the 2 application servers.

I intend to use Ansible as my configuration management tool to practice and work with the 5 nodes. 
Will also use ansible to do the provisioning 

## Details of the infrastructure
### OS Details:
CentOS 7.2

## NODES with IP details.
10.0.1.10 lbcer
10.0.1.11 dev01
10.0.1.12 dev02
10.0.1.13 db01
10.0.1.14 db02


## Next ... ?
Will update the README doc as I go along.


