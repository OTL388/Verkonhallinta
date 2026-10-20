
# Johdanto

Infrastructure as Code on infran määrittämistä ja hallintaa koodin avulla.


# Inventory

Inventory sisältää laitteet (ansible, attacker, branch-client, cadvisor, client1, db1, grafana, prometheus, r1, r2, r3, web1, zabbix) ja ne on luokissa seuraavasti: reitittimet (r1, r2, r3), asiakaskoneet (client1, attacker, branch-client), palvelimet (web1, db1), monitorointikoneet (prometheus, grafana, zabbix, cadvisor), hallinta (ansible), käyttäjäverkko (client1, attacker), palvelinverkko (web1, db1), toimipiste (branch-client), verkkolaitteet (reitittimet), linux laitteet (asiakaskoneet, palvelimet, monitorointikoneet, hallinta), ubuntu laitteet (client1, web1, db1, branch-client), node exporter (reitittimet asiakaskoneet, palvelimet).

Ryhmät auttavat laitteiden hallinnassa.

# Esimerkkiplaybookit

Playbook tekee yhteys testin. 
Tuloksista voidaan päätellä, ettei monitorointikoneissa ja reitittimissä ole ssh yhteyttä.

Playbookeissa käytetään seuraavia moduuleja: apt, file, get_url, unarchive, copy, shell, uri, debug, ja service.
Muuttujia on käytetty esim. node exportterin version valitsemiseen ja lataus url:n täydentämiseen dynaamisesti. Muuttujia on käytetty myös esim. tulostuksessa inventory_hostname, joka palauttaa palvelimen nimen tai jotai emt.
handelers-lohkoa käytetään 


# Oma playbook

Koodi ja suorituksen tulokset (web-palvelin ja/tai tietokantapalvelin).

# Vertailu

Käsin vs. automaatio.

# Yhteenveto

Opitut asiat.
