#cloud-config
packages:
  - squid
package_update: true
package_upgrade: true
runcmd:
  - cd /etc/squid/
  - rm squid.conf
  - wget https://raw.githubusercontent.com/steamme/squid/main/squid.conf
  - sudo systemctl restart squid
  - sudo ufw allow 'Squid'
