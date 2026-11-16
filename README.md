# Crypto — Releases

Installeurs et manifeste de mise à jour automatique (`latest.json`) de l'application Crypto.

**➜ [Télécharger la dernière version](../../releases/latest)** — la page indique quel fichier prendre selon votre système, et donne les empreintes SHA-256 pour vérifier votre téléchargement.

## Deux signatures à ne pas confondre

- Les **mises à jour** sont signées cryptographiquement (fichiers `.sig`). L'application refuse tout paquet dont la signature ne correspond pas à notre clé.
- Les **installeurs** ne portent pas de certificat Apple ni Microsoft. **Windows et macOS afficheront donc un avertissement au premier lancement**, et c'est attendu. Ne prenez pas l'absence d'avertissement pour une preuve d'authenticité : vérifiez l'empreinte SHA-256 publiée sur la page de la version.

## Ce que fait Crypto, et ce qu'il ne fait pas encore

Les messages sont chiffrés de bout en bout (X3DH + double cliquet). L'**anonymat réseau**, lui, exige trois relais Gotham sur trois réseaux distincts ; tant que ce n'est pas le cas, l'application affiche « Boîte aux lettres seule » et l'opérateur d'un relais peut observer qui échange avec qui. L'indicateur dans l'application dit la vérité — fiez-vous à lui.

## Code source

Binaires uniquement ici : le code de l'application reste privé. Le relais Gotham, lui, est libre sous AGPL — [0x9Angel/gotham-relay](https://github.com/0x9Angel/gotham-relay) — pour que n'importe qui puisse en faire tourner un et vérifier ce qu'il fait.

Un problème, une question : [signaler](https://github.com/0x9Angel/gotham/issues), ou écrire à **SoraCorporation@proton.me**.
