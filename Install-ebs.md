# Smart image renamer tbv foto's.


## Aanmaken virtualenv voor smart-image-renamer

````
mkvirtualenv image-rename
pip3 install smart-image-renamer
````

## Overschrijf deze versie met de laatste uit GitHub ivm bug-fixes (!)

````
cd /python/projects 
git clone https://github.com/ronakg/smart-image-renamer

cp /python/projects/smart-image-renamer/_version.py            /Users/esc21191/.virtualenvs/image-rename/bin
cp /python/projects/smart-image-renamer/smart-image-renamer.py /Users/esc21191/.virtualenvs/image-rename/bin
````

## Rename foto's !

````
workon image-rename
smart-image-renamer.py -h


cd /python/opzij/2018-04-24-Whirinaki-Forest-park

rm -rf /tmp/2018-04-24-Whirinaki-Forest-park
cp -R /python/opzij/2018-04-24-Whirinaki-Forest-park /tmp

smart-image-renamer.py -f {YYYY}{DD}{MM}-{hh}h{mm}-Whirinaki-Forest-{File}   /tmp/2018-04-24-Whirinaki-Forest-park
````

