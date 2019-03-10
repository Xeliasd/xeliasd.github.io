Stránka je kompilovaná s pouitím Jekyll v 3.7.4, 
keïe novšie verzie z Jekyll docs stránky nie sú plne kompatibilné s GitHub pages - tie beia na 3.7.4.
GitHub support mi po dlhotrvajúcich problémoch so zlyhávajúcimi buildami doporuèili pod¾a ich návodu preinštalova Jekyll.
Vïaka tomu som zistil, e bug opravenı v neskorších verziách stále robí problémy na github pages.
Konkrétne išlo o kombináciu | date_to_long_string: "ordinal" spolu s definíciou urèitej triedy. Teda ak na verzií 3.7.4 priradím triedu
a nastavím farbu/font tohto textu cez class="nieèo", u nemôem nastavi "ordinal".
Táto verzia jekyllu spúša kompiláciu cez "bundle exec jekyll serve"