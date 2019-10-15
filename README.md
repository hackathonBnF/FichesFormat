# Fiches Format

## Native FLAC
### Description
Le format FLAC (*Free Lossless Audio Codec*) est à la fois un format conteneur et un codec audio ouverts permettant une compression sans perte d’un flux LPCM.
Il s’agit d’un format adapté à une diffusion de type « streaming » qui est donc résilient aux altérations grâce à une structure en blocs. Chacun des blocs dispose d’une empreinte numérique embarquée.
### Sociabilité
Le format FLAC est très largement géré par les logiciels et matériels audiovisuels. Son adoption s’est développée à partir de 2017, date à partir de laquelle les nouvelles versions de la plupart des navigateurs internet le gèrent.
### Contenu
Un flux audio FLAC peut également être embarqué dans un format conteneur OGG. Une autre option, plus rare, est de l'embarquer dans un format conteneur Matroska.
### Organisme de maintenance et documentation de référence
Le format FLAC est maintenu par la fondation à but non lucratif Xiph.org.
Le site web officiel du format est https://xiph.org/flac/.
En outre, le projet CELLAR (https://datatracker.ietf.org/wg/cellar/charter/) vise à normaliser un format audiovisuel utilisant Matroska comme format conteneur, FFV1 comme codec vidéo et FLAC comme codec audio.
### Identifiants
|  Registre   |   Identifiant    |
| :------------| :------------- |
| Wikidata   |     [Q219848](https://www.wikidata.org/wiki/Q219848)     |
|   Bibliothèque du Congrès  |    [fdd000198](https://www.loc.gov/preservation/digital/formats/fdd/fdd000198.shtml) (version 1.1.2)   |
| PRONOM        |   [fmt/279](https://www.nationalarchives.gov.uk/PRONOM/fmt/279) (version 1.2.1)     |
### Caractéristiques techniques
La compression mise en oeuvre par le codec FLAC permet de réduire de 30 à 70% la taille d'un flux LPCM. Il s'agit d'une compression sans perte : si l'on encode un fichier WAVE en FLAC puis qu'on le décode à nouveau vers WAVE, le flux audio décodé est strictement équivalent (a la même empreinte numérique) que le fichier WAVE originel. *Note : afin de conserver les métadonnées RIFF d'origine dans le fichier FLAC, on veillera à employer l'option --keep-foreign-metadata à l'encodage et au décodage.*
### Outils d’analyse
La fondation Xiph.org développe également l’outil en ligne de commande "flac" (https://xiph.org/flac/documentation_tools_flac.html) qui permet d'encoder et de décoder des flux FLAC à partir de WAVE, WAVE 64, RF64 et AIFF et de valider la structure du flux FLAC.
L'outil d'analyse et d'extraction de métadonnées techniques est MediaInfo (https://mediaarea.net/fr/MediaInfo).
### Métadonnées internes
Le format FLAC permet d'embarquer des métadonnées internes aux formats Vorbis et ID3. L'outil metaflac (https://xiph.org/flac/documentation_tools_metaflac.html) permet d'éditer ces métadonnées. 
### Formats de métadonnées techniques
Le format MPEG-7 est le format de métadonnées techniques préféré par la BnF pour le format FLAC. Il s'agit d'un format de sortie natif de l'outil MediaInfo (https://mediaarea.net/fr/MediaInfo).
