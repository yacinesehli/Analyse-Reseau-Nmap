#  Analyse de Réseau Local avec Nmap et Zenmap

**Auteur :** Yacine SEHLI  
**Type :** Audit Réseau / Reconnaissance  
**Outils :** Nmap, Zenmap, Kali Linux  

---

##  Résumé du Projet
Ce projet présente une analyse complète d'un réseau local réalisée à l'aide des outils **Nmap** (CLI) et **Zenmap** (GUI). L'objectif était de découvrir les hôtes actifs, d'identifier les ports ouverts, de reconnaître les services (Fingerprinting) et les systèmes d'exploitation afin d'évaluer la sécurité du réseau.

##  Compétences Techniques
* **Scan de Ports :** Utilisation de `nmap -p` pour cartographier les ports TCP complets (0-65535).
* **Détection de Services :** Identification des versions précises (ex: Samba, Boa httpd, VoIP services).
* **Détection d'OS :** Fingerprinting de la stack TCP/IP pour identifier le système (Linux/VirtualBox).
* **Analyse Graphique :** Utilisation de Zenmap pour visualiser les résultats et la topologie.

##  Structure du Dépôt
* **`Rapport_Nmap_Zenmap.pdf`** : Le rapport complet généré en LaTeX, détaillant la méthodologie et l'analyse.
* **`evidence/`** : Captures d'écran des scans (CLI et GUI) prouvant les résultats.
* **`src/`** : Code source LaTeX du rapport.

##  Résultats Clés
L'analyse a révélé que la cible (192.168.1.1) expose plusieurs services critiques, notamment :
* **Partage de fichiers** (Ports 139, 445 - Samba)
* **Serveur Web** (Port 80 - Boa httpd)
* **VoIP** (Ports 2000 SCCP, 5060 SIP)

---
*Projet réalisé dans le cadre de mon apprentissage en cybersécurité.*