# Project
Šī programma ir izstrādāta, lai ģenerētu nejaušus cilvēku vārdus un ievietotu tos jaunā Excel failā, kas izveidots datorā. Pēc tam nosaukumi tiks pārveidoti par Morzes kodu, izmantojot šo vietni https://morsedecoder.com/ un arī ievietoti Excel failā (names.xlsl).


Lai ģenerētu nejaušus vārdus, es izmantošu Faker bibliotēku. Lai to ieladet vagag terminala uzrakstit (pip install faker). Importēšana pēc instalēšanas importēju Faker moduli savā Python skriptā( from faker import Faker). Faker bibliotēku var konfigurēt vajadzīgajai valodai un arī tam, kas jāģenerē, piemēram, adresēm, vārdiem un e-pastiem.


Openpyxl Bibliotēku izmantošu arī darbam ar Excel failiem. Šajā projektā šī bibliotēka izveidos un uzglabās ģenerētos vārdus un to nozīmi Morzes kodā. Katru reizi pēc koda izmantotie vārdi un to kodi tiks ģenerēti vienā un tajā pašā nosaukumu failā, dzēšot iepriekšējos.


Tiks izmantota arī selenium bibliotēka lai atvērtu vietni https://morsedecoder.com/, izmantojot pārlūku Chrome. Izmantojot .selēnu. Es varu atrast pogu Accept all & visit the site. Atrodiet vietu, kur es varu ievietot nosaukumus no faila names un pēc tam atrodiet vārdus, kas pārveidoti par Morzes kodu.


Kods strāda tā:


Pirmkart importejam visas vajadzigas Selenium,Openpyxl un Faker. Veidojas workbooks(excel fails) kura pirma rinda, pirma un otra kolonna ir tie nosaukumi "Name" un "Morse Codet name".Pec tam veido 100 random vārdus kollona A.
Pēc tam atveras vietne https://morsedecoder.com/ kura parveidos veidotus random vārdus morzes koda.Un Pēc tam ievieto morzes koda vārdus kollonā B un saglaba šo visu faila (names.xlsl). Fails names bus veidots vienu reiz bet 
pec katras koda izmontošanas bus veidoti citi random vārdi un tie morzes kodi.
