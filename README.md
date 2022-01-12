![Github logo](/dwonload.png)
)


------------------

### Mitä versiohallinnalla tarkoitetaan?
Versionhallinnalla tarkoittaa menetelmää, joka säilöö tietoa ja siihen tehtyjä muutoksia.


Git on hajautetun versiohallinnan menetelmä jossa ideana on tarjota säilytyspaikka käytettävälle tiedolle ja pitää kirjaa tietoon tehdyistä muutoksista. Alunperin Git:n on kehittänyt suomalainen [Linus Thorvalds](https://fi.wikipedia.org/wiki/Linus_Torvalds).

### Mikä [GitHub](https://github.com/) on?

*GitHub* mahdollistaa myös saman tiedon parissa työskentelyn eri tietokoneilta.


---------------

Git tietojen määrittäminen:
- Git versiohallinnan ottaminen käyttöön työkansiossa: ```git init```   
- Git käyttäjänimen määrittäminen: ```git config user.name```   
- Sähköpostiosoitteen määrittäminen: ``` git config --global user.email "erkki.esimerkki@example.com" ```  
- Git tietojen näyttäminen: ```git config --list --global```    

Git työskentelyn peruskomentoja:
- Tiedon tuottaminen ja muokkaaminen Git työkansiossa   
- Tiedon lisääminen Git indeksiin: ```git add b.txt``` tai ```git add .```  
- *Commit:n* luominen indeksissä olevista tiedoista: ```git commit -m "Commit viesti"```   
- *Git commit:n* listaaminen: ```git log``` tai ```git log --oneline``` 
- *Git* tilan tarkastminen: ```git status```   

**Github <-> Git työskentely:**

Työhakemiston synkronoiminen *GitHub:n*:
- Paikallisen työkansion kytkeminen GitHub repositorioon:   
 ```git remote add origin https://github.com/GitHubTunnus/GitHubRepositorio.git```   
- Etärepositorio kytköksen tarkistaminen: ```git remote -v```   
- Paikallisen työkansion tietojen puskeminen *GitHub*:n:``` git push -u origin master```   

*GitHub*:a olevien tietojen synkronoiminen paikalliseen työkansioon:
- *GitHub* repositorion ja paikallisen työkansion tilenteen erojen päivittäminen: ```git fetch```  
- Tietojen lataaminen *GitHub* repositoriosta paikalliseen työkansioon: ``` git pull ```  

Git *fork*:n liittyviä Git komentoja
- *Upstream remoten* lisääminen paikalliseen Git työhakemistoon:   
```git remote add upstream git://github.com/GitHubTunnus>/GitHubRepositorio.git>```     
- *Upstream remoten* tietojen synkronoiminen Giot työhakemistoon: ```git fetch upstream```   

**Haarat eli *branch*:t**:

Git haara (*branch*) on toiminallisuus joka mahdollistaa haarassa olevien tietojen muuttamisen ilman että muutoksilla on vaikutusta työkansion muihin tietoihin.

Git haaroihin liittyvä työskentely:
- Git haarojen listaaminen: ```git branch```    
- Uuden haaran lisääminen: ```git branch haaran_nimi``` tai ```git checkout haaran_nimi```   
- Haaran tietojen yhdistäminen *master* päähaaraan: ```git merge haaran_nimi```   
- Haaran poistaminen: ```git branch -d uusibranch```

--------------------

