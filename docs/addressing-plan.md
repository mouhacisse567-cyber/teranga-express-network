# Plan d'adressage

| Site | VLAN | Nom | Réseau | Passerelle |
|---|---|---|---|---|
| Siège | 10 | Direction | 10.10.10.0/24 | 10.10.10.1 |
| Siège | 20 | Opérations | 10.10.20.0/24 | 10.10.20.1 |
| Siège | 30 | Serveurs | 10.10.30.0/24 | 10.10.30.1 |
| Siège | 40 | Invités | 10.10.40.0/24 | 10.10.40.1 |
| Siège | 99 | Gestion | 10.10.99.0/24 | 10.10.99.1 |
| Thiès | 10, 40, 99 | Employés, invités, gestion | 10.20.10.0/24, 10.20.40.0/24, 10.20.99.0/24 | .1 de chaque réseau |
| Saint-Louis | 10, 40, 99 | Employés, invités, gestion | 10.30.10.0/24, 10.30.40.0/24, 10.30.99.0/24 | .1 de chaque réseau |

Liens entre sites : 172.16.0.0/30 (Siège-Thiès), 172.16.0.4/30 (Siège-Saint-Louis), 172.16.0.8/30 (Thiès-Saint-Louis)

Serveur du siège : 10.10.30.10