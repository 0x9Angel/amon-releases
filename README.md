# Amon Messenger — Releases

Installeurs et canal de mise à jour d'**Amon Messenger**, la messagerie qui s'appelait Crypto avant la version 2.5.0. Chaque application installée lit ici le manifeste de mise à jour automatique (`latest.json`).

**➜ [Télécharger la dernière version](../../releases/latest)** — la page indique quel fichier prendre selon votre système, et donne les empreintes SHA-256 pour vérifier votre téléchargement.

Ce dépôt s'appelait `crypto-releases`. GitHub redirige les anciennes adresses vers lui, y compris celle que lisent les applications déjà installées pour trouver leurs mises à jour.

## Deux signatures à ne pas confondre

- Les **mises à jour** sont signées cryptographiquement (fichiers `.sig`). L'application refuse tout paquet dont la signature ne correspond pas à notre clé.
- Les **installeurs** ne portent pas de certificat Apple ni Microsoft. **Windows et macOS afficheront donc un avertissement au premier lancement**, et c'est attendu. Ne prenez pas l'absence d'avertissement pour une preuve d'authenticité : vérifiez l'empreinte SHA-256 publiée sur la page de la version.

## Ce que fait Amon Messenger, et ce qu'il ne fait pas encore

Les messages sont chiffrés de bout en bout (X3DH + double cliquet). L'**anonymat réseau**, lui, exige des relais du réseau Amon tenus par au moins trois opérateurs indépendants, sur des réseaux distincts ; tant que ce n'est pas le cas, l'application affiche « Boîte aux lettres seule » et l'opérateur d'un relais peut observer qui échange avec qui. L'indicateur dans l'application dit la vérité — fiez-vous à lui.

## Code source

Binaires uniquement ici : le code de l'application reste privé. Le réseau Amon, lui, est libre sous AGPL, pour que n'importe qui puisse faire tourner un relais et vérifier ce qu'il fait : son code est dans [0x9Angel/amon-network](https://github.com/0x9Angel/amon-network), les installeurs et les binaires du relais dans [0x9Angel/amon-relay](https://github.com/0x9Angel/amon-relay).

Un problème, une question : [signaler](https://github.com/0x9Angel/amon-network/issues), ou écrire à **SoraCorporation@proton.me**.
