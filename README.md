## It is a copy of Drupal VM project with some customizations and Drupal 8.2.5
[Drupal VM](https://www.drupalvm.com/)

## Quick start
1. Install the last stable version of Virtualbox(5.1+)
2. Install the last stable version of Vagrant (1.9.x+)
3. Install hostupdater plugin for Vagrant: `vagrant plugin install vagrant-hostsupdater`
4. Clone this repository
5. vagrant up

Clean Drupal 8.2.5 will be available via http://drupal.dev.

For more details check [Drupal VM](https://www.drupalvm.com/)

## Requirements
1. Virtualbox 5.1
2. Vargant 1.9.x

## License

This project is licensed under the MIT open source license.

## FAQ
### Q: How to upgrade virtualbox from 5.0 to 5.1 on Ubuntu 16.04
### A:
   
```
   sudo service virtualbox stop
   
   sudo apt remove virtualbox-\*
   sudo apt purge virtualbox-\*
   
   Remove all modules from this command`s output:
   cd / && sudo find -iname "vbox"
   
   sudo sh -c 'echo "deb http://download.virtualbox.org/virtualbox/debian xenial contrib" >> /etc/apt/sources.list.d/virtualbox.list'
   wget -q https://www.virtualbox.org/download/oracle_vbox_2016.asc -O- | sudo apt-key add -
   sudo apt update
   sudo apt install virtualbox-5.1
   
   sudo /sbin/rcvboxdrv setup
```
   