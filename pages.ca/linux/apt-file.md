# apt-file

> Busca arxius en paquets APT, incloent els que encara no s'han instal·lat.
> Més informació: <https://manned.org/apt-file.1>.

- Actualita les metadades de la base de dades:

`sudo apt update`

- Busca paquets que continguin l'arxiu o ruta especificada:

`apt-file {{search|find}} {{ruta/al/arxiu}}`

- Mostra el contingut del paquet especificat:

`apt-file {{show|list}} {{nom_paquet}}`

- Busca paquets que igualin l'expressió regular donada en `patró`:

`apt-file {{search|find}} --regexp {{expressió_regular}}`
