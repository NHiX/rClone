# rClone
exemples et utilisation de rClone

rClone est un utilitaire multi-plateforme utilisable en ligne de commande
qui va permettre de sauvegarder, chiffrer, rapatrier des fichiers depuis differentes plateformes Cloud, tels que:

1Fichier, Amazon S3, Box, Dropbox, Google Drive, Hubic, Mega ou encore OneDrive

1/ Copie d'un fichier vers une plateforme cloud (OneDrive)

<code>rclone config</code>

une fois configurer avec le service désiré, il y a juste à passer la commande:

<code>rclone copy monfichier.extension nomduservice:</code>

Vous pouvez spécifier un chemin d'accès après les ":" :

<code>rclone copy monfichier.extension nomduservice:/monrepertoire/</code>


2/ Utilisation de rClone dans le cadre d'un "montage" d'un volume Google Drive sur répertoire

<code>rclone config</code>

une fois le service configuré, on peut "monter" celui-ci en tant que filesystems:

<code>rclone mount --daemon nomduservice: /home/utilisateur/repertoire</code>

3/ Montage d'un repertoire Cloud chiffré

<code>rclone config</code>
