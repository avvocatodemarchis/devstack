# Devstack Essentials

We setup this lab with as a single machine OpenStack deployment.

## Start OpenStack Deployment
- open a puTTY session to `devstack.corp.local`
- use the credentials:
	- _viouser_/VMware123
- go to the `/home/viouser/devstack` folder
- run `./stack.sh`
- it takes around 20 minutes for the stack.sh script to complete.
- once the script is done, you can start using Devstack (see Credentials section below)

## Stop the OpenStack Deployment
- **NOTE: do the follwoing steps BEFORE powering off the `devstack.corp.local machine`**
- open a puTTY session to devstack.corp.local
- use the credentials:
	- _viouser_/VMware123
- cd in `/home/viouser/devstack` folder
- run `./unstack.sh`


## Environment
### Enabled Openstack Services
	- neutron
	- heat
	- ceilometer
	- gnocchi
	- aodh

### OpenStack Credentials
| Type | Username | Password |
| --- | --- | --- |
| Admin Account | _admin_ | vtsu
| User Account | _demo_ | vtsu

### Openstack Command clients
- open a puTTY session to `devstack.corp.local`
- use the credentials:
  - _viouser_/VMware123
- cd in `/home/viouser/devstack` folder
  - run `source openrc`
- By default, sourcing `openrc` grants access as the _demo_ user.

### Devstack Host Machine Credentials
- hostname: `devstack.corp.local`
- IP: `192.168.110.100`
- login: _viouser_
- password: VMware123
