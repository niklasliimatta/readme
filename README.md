![Git ja GitHub](https://www.google.com/search?q=github+logo&sxsrf=AOaemvIqFUokJ48SCGU8e1r-OpZ0ZNxaNw:1641987010037&tbm=isch&source=iu&ictx=1&vet=1&fir=O1ZHcIfZkHZqiM%252CHIAMPS7ac5hM_M%252C_%253BKq4l3mSBVj08zM%252CH8p6HHzcTglWAM%252C_%253BF4N7nNsmAvS0zM%252CTXCcjLeV5gKBaM%252C_%253BECqRgpVdvbaoQM%252C2RrOa4w_PYanyM%252C_%253BfLKD7QptF_vjyM%252CH8p6HHzcTglWAM%252C_%253BkA2-FqAeptEp1M%252CaZMTzBMUx1GvGM%252C_%253BpofdzE5TmkauXM%252C_ryaMNeKRdf30M%252C_%253Br2oa1LiSCrkGlM%252CoC1d98N8B9Q4cM%252C_%253B58ZUu1xG6gAEOM%252CryGNGNSzKs_dRM%252C_%253B_OjrNiGLxhfxQM%252C6c2yz7gdNvDU7M%252C_%253BdO1l3HgJbssG8M%252CgwkaSaXL7ezQZM%252C_%253BZs51aR2puky1QM%252C2RrOa4w_PYanyM%252C_%253BJdCuiEb92j8WmM%252ChOKru3WHzG-XsM%252C_%253BDGVHjhSEPkJgLM%252Ct7BPFRnhuadZ4M%252C_%253BuNiYLmnMJypvEM%252CuxEPehlkPHmQdM%252C_&usg=AI4_-kS0Qm7PtXxy4H2rViZuTBHUIBYy6Q&sa=X&ved=2ahUKEwjAxNWjjqz1AhUtlYsKHQWGC3kQ9QF6BAgmEAE#imgrc=ECqRgpVdvbaoQM)


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

