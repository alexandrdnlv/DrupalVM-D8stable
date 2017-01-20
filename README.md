## It is a copy of Drupal VM project with some customizations and Drupal 8.2.5
[Drupal VM](https://www.drupalvm.com/)

## Requirements
1. Virtualbox 5.1
2. Vargant 1.9.x

*How to upgrade virtualbox from 5.0 to 5.1 on Ubuntu 16.04*
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
## License

This project is licensed under the MIT open source license.
