Str�nka je kompilovan� s pou�it�m Jekyll v 3.7.4, 
ke�e nov�ie verzie z Jekyll docs str�nky nie s� plne kompatibiln� s GitHub pages - tie be�ia na 3.7.4.
GitHub support mi po dlhotrvaj�cich probl�moch so zlyh�vaj�cimi buildami doporu�ili pod�a ich n�vodu prein�talova� Jekyll.
V�aka tomu som zistil, �e bug opraven� v neskor��ch verzi�ch st�le rob� probl�my na github pages.
Konkr�tne i�lo o kombin�ciu | date_to_long_string: "ordinal" spolu s defin�ciou ur�itej triedy. Teda ak na verzi� 3.7.4 prirad�m triedu
a nastav�m farbu/font tohto textu cez class="nie�o", u� nem��em nastavi� "ordinal".
T�to verzia jekyllu sp���a kompil�ciu cez "bundle exec jekyll serve"