Devstack Essentials

To start the OpenStack Cloud 
	- open a putty session to devstack.corp.local (viouser/VMware123)
	- cd in /home/viouser/devstack
	- run ./stack.sh
	- it takes around 20 minutes for the stack.sh script to complete.

Openstack Services Enabled
	- neutron
	- heat
	- ceilometer
	- gnocchi
	- aodh 

To stop the OpenStack Cloud (NOTE: do this before powering off the devstack.corp.local machine)
	- open a putty session to devstack.corp.local
	- cd in /home/viouser/devstack
	- run ./unstack.sh

Devstack Host Machine Credentials
	hostname: devstack.corp.local
	IP: 192.168.110.100
	login: viouser
	password: VMware123

OpenStack Cloud Credentials
 ___ 
| 1 |user: admin
|   |password: vtsu
|---|--------------------------
| 2 |user: demo
|___|password: vtsu

To use Openstack Command clients
	- open a putty session to devstack.corp.local
	- cd in /home/viouser/devstack
    - run 'source openrc'

This is your host IP address: 192.168.110.100
This is your host IPv6 address: fe80::250:56ff:fe02:a62
Horizon is now available at http://192.168.110.100/dashboard
Keystone is serving at http://192.168.110.100/identity/
The default users are: admin and demo
The password: vtsu