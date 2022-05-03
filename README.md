## Netcup-Keepalived

WIP!

Set up the latest or a specific version of [Keepalived](http://www.keepalived.org/) in Debian-like systems combined with SOAP Scripts for the Netcup API.

Credits go to @Oefenweb on which the keepalived role is based.

#### Requirements
- :exclamation: Failover IPv4 https://www.netcup.de/bestellen/produkt.php?produkt=1073
- :information_source: Failover IPv6 https://www.netcup.de/bestellen/produkt.php?produkt=1074

#### Install Roles

```sh
 $ ansible-galaxy install -r requirements.yml
 ```

#### Example Inventory

See [Inventory](inventory.yml) for example values. Please note that IPv4 Failover IP is a hard requirement and must be set, but IPv6 Failover IP can be left blank.

#### Example Call

```sh
 $ ansible-playbook -i inventory.yml site.yml
 ```
