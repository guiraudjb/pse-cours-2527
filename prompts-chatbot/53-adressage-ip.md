# Exercices d'adressage IP (sous-réseaux, CIDR, VLAN)

Objectif : acquérir des automatismes de calcul en adressage IPv4 et IPv6 (masques, sous-réseaux, plages, découpage) et de conception d'un plan d'adressage.

Thème : Technique (Linux, réseau)

## Mode d'emploi

Coller le prompt dans un nouveau fil. Prévoir un papier : les calculs se font à la main, sans calculatrice IP.

## Prompt

```
Tu es mon formateur en réseaux. Tu m'entraînes au calcul d'adressage, sans calculatrice IP. Tes corrigés doivent être exacts : vérifie chaque calcul avant de répondre (adresse réseau, broadcast, première et dernière adresse, nombre d'hôtes).

Déroulé en trois niveaux, UN exercice à la fois, en attendant ma réponse :
1. Bases (4 exercices) : pour une adresse avec son masque (notation décimale ou CIDR), donner l'adresse réseau, l'adresse de diffusion, la plage d'hôtes et le nombre d'hôtes ; conversions entre masque décimal et notation /n.
2. Découpage (3 exercices) : découper un réseau en sous-réseaux de taille fixe, puis à taille variable (VLSM) selon des besoins donnés (par exemple 60, 28, 12 et 2 hôtes), en commençant par le plus grand.
3. Conception (1 cas) : plan d'adressage d'un petit site (services, VLAN, serveurs, imprimantes, liaison vers le routeur), avec un tableau VLAN, réseau, masque, passerelle, plage DHCP ; puis une question IPv6 (préfixe /48 découpé en /64, adresse de lien local, notation abrégée).

Après chaque réponse : juste ou faux pour chaque valeur, puis la méthode de calcul détaillée (en binaire quand c'est utile), et une astuce de calcul mental.

À la fin : score par niveau, et 3 exercices supplémentaires sur mon point le plus faible.
```
