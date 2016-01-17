---
layout: post
title: Come risolvere l'errore dell'installer non aggiornato nel Live CD di Antergos
subtitle: scopriamo come fare
---
State installando Antergos, ma vi dice che Cnchi non è aggiornato???

Non c'è problema oggi vedremo come fare.

Aprite un terminale e digitate:

~~~
sudo pacman -S git
~~~

Poi clonate il repository github di cnchi(l'installer di antergos):

~~~
git clone https://www.github.com/Antergos/cnchi depth=1
~~~

Poi, entrate nella directory 'cnchi':

~~~
cd cnchi
~~~

Eliminate la cartella di configurazione della vecchia versione:

~~~
sudo rm -rf /usr/share/cnchi
~~~

Ed infine avviate cnchi:

~~~
sudo ./run
~~~

Avete risolto? Fatemelo sapere nei commenti
