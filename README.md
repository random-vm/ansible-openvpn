Role Name
=========

openvpn

- Builds remote access openvpn server on Debian 9
- Generates access keys under /etc/openvpn/easy-rsa/clients/
- Configured with ability to revoke certificates with /usr/share/easy-rsa/revoke-full username

Requirements
------------

- Debian 9 

Usage
-----

Example run command:

     ansible-playbook openvpn.yml -i '<PublicIP>,' \
                                     -e 'ip_address=0.0.0.0' \ #your public IP or your VPN server
                                      -u $SSHUSER \
                                      --sudo -vvvv

License
-------

     GNU General Public License family

Author Information
------------------
     MTMcGrath
