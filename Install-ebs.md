# Smart image renamer tbv foto's.


## Aanmaken virtualenv voor smart-image-renamer

````
mkvirtualenv image-rename
pip3 install smart-image-renamer
````

## Overschrijf deze versie met de laatste uit GitHub ivm bug-fixes (!)

````
cd /python/projects 
git clone https://github.com/fbascheper/smart-image-renamer

cp /python/projects/smart-image-renamer/_version.py            ~/.virtualenvs/image-rename/bin
cp /python/projects/smart-image-renamer/smart-image-renamer.py ~/.virtualenvs/image-rename/bin
````

## Rename foto's !

````
workon image-rename
smart-image-renamer.py -h


cd /tmp
rm -rf /tmp/2018-*
cp -R /fotos/2018/2018-04-18-Lokatie-onbekend /tmp

smart-image-renamer.py -f {YYYY}{MM}{DD}-{hh}h{mm}-Lokatie-onbekend-{File}   /tmp
````

