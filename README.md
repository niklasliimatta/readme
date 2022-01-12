Mitä versiohallinnalla tarkoitetaan?
Versionhallinnalla tarkoittaa menetelmää, joka säilöö tietoa ja siihen tehtyjä muutoksia.

Versionhallinta mahdollistaa tiedon varmuuskopioinnin. Varmuuskopiot (commitit) sisältävät sekä tiedon nykyisen, että aikaisemman tilan.
Versiohallinta (GitHub:n kautta) mahdollistaa tiedon jakamisen muille, sekä osallistumisen muiden projekteihin.

Git on hajautetun versiohallinnan menetelmä jossa ideana on tarjota säilytyspaikka käytettävälle tiedolle ja pitää kirjaa tietoon tehdyistä muutoksista.  
  
GitHub mahdollistaa myös saman tiedon parissa työskentelyn eri tietokoneilta.

Git versiohallinnan ottaminen käyttöön työkansiossa: git init
Git käyttäjänimen määrittäminen: git config user.name
Sähköpostiosoitteen määrittäminen: git config --global user.email "erkki.esimerkki@example.com"
Git tietojen näyttäminen: git config --list --global
Git työskentelyn peruskomentoja:

Tiedon tuottaminen ja muokkaaminen Git työkansiossa
Tiedon lisääminen Git indeksiin: git add b.txt tai git add .
Commit:n luominen indeksissä olevista tiedoista: git commit -m "Commit viesti"
Git commit:n listaaminen: git log tai git log --oneline
Git tilan tarkastminen: git status

Git haara (branch) on toiminallisuus joka mahdollistaa haarassa olevien tietojen muuttamisen ilman että muutoksilla on vaikutusta työkansion muihin tietoihin. 
Git haarojen listaaminen: git branch
Uuden haaran lisääminen: git branch haaran_nimi tai git checkout haaran_nimi
Haaran tietojen yhdistäminen master päähaaraan: git merge haaran_nimi
Haaran poistaminen: git branch -d uusibranch
