Ympäristön tarkoitus.




1.1
r1 - router1?
r2 - router2?
r3 - router3?
client1 - käyttäjä
attacker -
web1 -
db1 - database1
branch-client -
ansible -
prometheus -
grafana - 
zabbix - 


1.2
KAAVIO! esim:
                     Branch Office
                     10.10.30.0/24

                  branch-client
                        |
                       r3
                        |
                 10.255.23.0/30
                        |
                       r2
          --------------+--------------
          |                           |
          |                           |
     10.10.20.0/24              10.10.99.0/24
        Server LAN             Management LAN

      web1     db1        ansible
                            grafana
                            prometheus
                            zabbix

                        |
                 10.255.12.0/30
                        |
                       r1
                        |
                 10.10.10.0/24
                    User LAN

               client1
               attacker



1.3 - IP:t
Verkko - Tarkoitus - Yhdyskäytävä
10.10.10..0/24 -
10.10.20.0/24 -
10.10.30.0/24 -
10.10.99.0/24 -
10.255.12.0/30 -
10.255.23.0/30 -

1.4 


