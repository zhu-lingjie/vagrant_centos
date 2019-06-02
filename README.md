# vagrant_centos

The image came with ubuntu for vagrant is just awesome, while I mostly work with redhat, I built the following centos environment. 

host [ mac ] : 
- mgmt server, install ansible and can ssh into all the ohter hosts 
- lb, loadbalancer for web servers 
- web[12], two web servers 
- db, datbase server
- app, one application server


After lanuching: 
1. The centos machines set passwordauthentication to false, I comply that, 
    - copy all the ssh key over
    
2. The synced folder mount errores, from github 
https://github.com/geerlingguy/packer-centos-7/issues/18

`vagrant plugin install vagrant-vbguest`
however the process become very slow, hopefully in future, the boxes will include the features. 
