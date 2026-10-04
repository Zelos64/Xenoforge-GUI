## A télécharger / installer vous-même
Pour l'executable FFMPEG, il est disponible sur son site officiel : https://ffmpeg.org/download.html

Pour l'exécutable XbTool : https://github.com/AlexCSDev/XbTool
Pour l'exécutable XbxDETool : https://github.com/Nenkai/XbxDeTool

## Déjà présents
Pour le fichier  opus.dll :
	vous pouvez le retrouver à cette adresse : https://packages.msys2.org/packages/mingw-w64-x86_64-opus
	Descendez jusqu'à "file" et cliquer sur le lien miroir commençant par "https://mirror.msys2.org/mingw/..."

Pour l'exécutable nopus :
	Installez MSYS2 https://www.msys2.org/
	Une fois installé et lancé, entrez la commande suivante : pacman -S mingw-w64-ucrt-x86_64-gcc make mingw-w64-ucrt-x86_64-opus
	Validez avec Y chaque fois que c'est demandé
	Installez git avec cette commande : pacman -S git
	Puis la commande : git clone https://github.com/conhlee/nopus.git
	cd nopus
	make LDFLAGS="-l:libopus.a -lm -static"
	Retrouvez l'exécutable dans C:\msys64\home\%Username%\nopus