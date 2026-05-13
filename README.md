🧪 LAB 1 : Mise en place du lab (Mobexler + snapshot CLEAN)

Cours : Sécurité des applications mobiles

1. 📘 Glossaire (définitions rapides)
OVA : fichier contenant une machine virtuelle prête à être importée
VM : environnement virtuel simulant un ordinateur
Mobexler : plateforme de test pour sécurité mobile
ADB : outil de communication avec Android
Snapshot : sauvegarde d’un état système
USB passthrough : accès USB depuis la VM
2. 🎯 Objectifs pédagogiques
Installer Mobexler
Vérifier la connectivité réseau
Connecter un appareil Android
Créer un snapshot CLEAN
3. ⚙️ Prérequis
VirtualBox ou VMware Workstation
PC (Windows i5 suffisant)
Internet
Smartphone Android (optionnel)
4. 📥 Étape 1 — Télécharger Mobexler
🔗 Capture 1 — Téléchargement

https://images.openai.com/static-rsc-4/4Wmn6TCHdoOLqyQv0trcrEJulg3tF_fDBMpIm8SFKemO-ekCstgnTl3BZrci0TGTK9LGSuluJM6MHqK1r8QSiNkPDTbguvViJyDa5jS4SIPRioJWrmwrytYza6mS7oCaCOWd4aXRzEe6n2F6_UkWnD1-dCEFED_tQK3WPGhGqZMTRyJnm5MA4DE7uB0rc0i0?purpose=fullsize

📌 Résultat :

fichier .ova téléchargé
5. 💻 Étape 2 — Importer l’OVA
🔗 Capture 2 — Import OVA

https://images.openai.com/static-rsc-4/5qRelLeco_pCPPz0tzrbSY4xtoMW7ohcy9XZvIAU8h1lRkXS_klvZgo_BWFDFL6FlX8PI4iWaxV2MkGLBDJmoH678cMALsDJ2kTwVxAEgNQbE4jBMYqt31rcZhrs4jGmOQUimofDSZ0Tv1IHqKWCqTMIfyEQnVmXojlUS_5fFRkEBBZC8Jhm3pYGhD2YI1n6?purpose=fullsize

📌 Résultat :

VM visible dans VirtualBox
6. 🚀 Étape 3 — Premier démarrage + connexion
🔗 Capture 3 — Bureau Mobexler

https://images.openai.com/static-rsc-4/HonT6wcuQ8EWPXbW4BrAsboUUnqMDhTFYXEBuBGmerDo9MFJaiYNueezVtA0sCZZWCbnkeoR6Ck8tZnbgRKu23OlGOMUm3or3L79RFaAXbTlZzErfiSJ1R5XyW9-GqighHTJZD2hHqfLMtVzReJACz0jJ-M5HsMIUUzrBrjumetVKAeZcVA0inxTtvQHIRz_?purpose=fullsize

📌 Résultat :

VM démarre correctement
bureau affiché
7. 🌐 Étape 4 — Vérifier le réseau
Commandes :
ip a
ping -c 4 google.com
🔗 Capture 4 — IP

https://images.openai.com/static-rsc-4/ZNEjV2NHfuUL1LIfwTImR2ZguO9jfGqejJRBFGZxj-EnljZDOYfRMtplsPkQjE88Xa_nmUKxlpqXCv77dtwq9f8nwF-vLbKVabq4pTcFuBzzR5509m5SUL6EotwgHLeznzw8fmYA-1tngt7znnc9o9THo-2MV7b7T2JWs8blUzjIDDT-j7W35dGWNS6vurCB?purpose=fullsize

🔗 Capture 5 — Ping

https://images.openai.com/static-rsc-4/OYa6noQgFR2E6dtZLM5FJ5-dqGNX7n1bFhx8NVWUJYVeFpSqw2AkLiyvY0TP7vhUHGviDQMb3YsnQKOP3zfgBcDV-5jorViCIsGzugbw5_5Ffq1cM0Ud4Kl0BltpTdQJ_4iKR2_MwwQdqhkUAmFh6H4MePXHAdft_EIKLDMFLErDSy42CwDI0yjLiYD3KakZ?purpose=fullsize

📌 Résultat attendu :

IP affichée
Ping OK
8. 💾 Étape 5 — Snapshot CLEAN
🔗 Capture 6 — Snapshot

https://images.openai.com/static-rsc-4/IBuVqc7HV6DVIfcgXvw-HJt8vqK7kXFE4uFhLR_72AdxTuOm4mtBBZWZjSt8lCY17TFQCi4ua8c6Q2VYgJMOQFCVBQz7mF8ycoott2keXxVDVpI39GcFJk9R1hy4V1ngaA-OeH_Gs-YGnsB1DNCgAYBoKG3UflHz6HUp8aBHYmGqo5KSDT17J64rDrV-z62m?purpose=fullsize

📌 Résultat :

Snapshot nommé CLEAN créé
9. 📱 Étape 6 — Préparer la cible Android
🔹 Option A — Smartphone (recommandé)
A1 — Activer USB debugging
🔗 Capture 7 — Developer options

https://images.openai.com/static-rsc-4/28LcNG76rjiRWpjEeOVEnGG6EvDsaaGRyMLlGu0vpcBNuZtWujgpafoF6Q5jGkNCNVBQ1PL9OEkNXoZkAfGD0VljDCD5MDZdEOvNiLgWSJ0v0IR1cA-Qr7FuN0Er80DviCrchxXcDNk7FqwsKYWl55qxb0nxu_DKigebUcF5OwfG1FOU-qoPCmBqRiT-SFs1?purpose=fullsize

A2 — USB passthrough

👉 Dans VirtualBox :

Devices → USB → sélectionner téléphone
A3 — Vérifier ADB
Commandes :
adb version
adb devices
🔗 Capture 8 — ADB

https://images.openai.com/static-rsc-4/M9arjk5QzgYo9mkKExjNItpdPVsfrZEX4OMkx6CgWw4lamkzBY9sFklYTusWD1vBw16Uy9U9kLjIDdsU5I-vCmy33720qGeAkOLbX47uEdmB-Ap32AqXzPTOL6OWSn0uOIYMlZwvFYR8wIachhgITuGtIMnbAtqf5hHX9458ootkVy9wIKVGZEqrHIABZowo?purpose=fullsize

📌 Résultat attendu :

List of devices attached
XXXX	device
🔧 Dépannage
unauthorized → accepter popup téléphone
aucun device :
adb kill-server
adb start-server
adb devices
