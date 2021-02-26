# rClone
exemples et utilisation de rClone

rClone est un utilitaire multi-plateforme utilisable en ligne de commande
qui va permettre de sauvegarder, chiffrer, rapatrier des fichiers depuis differentes plateformes Cloud, tels que:

1Fichier, Amazon S3, Box, Dropbox, Google Drive, Hubic, Mega ou encore OneDrive

1/ Copie d'un fichier vers une plateforme cloud (OneDrive)

<code>rclone config</code>

une fois configurer avec le service désiré, il y a juste à passer la commande:

rclone copy monfichier.extension nomduservice:

Vous pouvez spécifier un chemin d'accès après les ":" :

rclone copy monfichier.extension nomduservice:/monrepertoire/


3/ Utilisation de rClone dans le cadre d'un "montage" d'un volume Google Drive sur répertoire

rclone config

