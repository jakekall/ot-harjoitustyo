# BrickBreaker-peli

Yksinkertainen Arkanoid-tyylinen peli satunnaisesti generoitavilla tasoilla.

## Dokumentaatio
[Käyttöohje](https://github.com/JakeKallioniemi/ot-harjoitustyo/blob/master/dokumentaatio/kayttoohje.md)  
[Vaatimusmäärittely](https://github.com/JakeKallioniemi/ot-harjoitustyo/blob/master/dokumentaatio/vaatimusmaarittely.md)  
[Arkkitehtuurikuvaus](https://github.com/JakeKallioniemi/ot-harjoitustyo/blob/master/dokumentaatio/arkkitehtuuri.md)  
[Testausdokumentti](https://github.com/JakeKallioniemi/ot-harjoitustyo/blob/master/dokumentaatio/testaus.md)  
[Työaikakirjanpito](https://github.com/JakeKallioniemi/ot-harjoitustyo/blob/master/dokumentaatio/tyoaikakirjanpito.md)  

## Releaset

[Viikko 5](https://github.com/JakeKallioniemi/ot-harjoitustyo/releases/tag/viikko5)  
[Viikko 6](https://github.com/JakeKallioniemi/ot-harjoitustyo/releases/tag/viikko6)  
[Loppupalautus](https://github.com/JakeKallioniemi/ot-harjoitustyo/releases/tag/loppupalautus)

## Komentorivitoiminnot

**HUOM!** Kaikki listatut komennot tulee suorittaa BrickBreaker-kansion sisällä eikä juurikansiossa.

### Käynnistys

```
mvn compile exec:java -Dexec.mainClass=brickbreaker.Main
```

Käynnistää ohjelman.

### Suoritettavan jar-tiedoston luonti

```
mvn package
```

Luo _BrickBreaker-1.0-SNAPSHOT.jar_ nimisen jar-tiedoston hakemistoon _target_.

### Testaus

```
mvn test
```

Suorittaa JUnit testit.


```
mvn jacoco:report
```

Luo HTML-muotoisen JaCoCo testikattavuusraportin, jota voi tarkastella avaamalla tiedoston _target/site/jacoco/index.html_ selaimella.

### JavaDoc

```
mvn javadoc:javadoc
```

Luo JavaDocin, jota voi tarkastella  avaamalla tiedoston _target/site/apidocs/index.html_ selaimella.

### Checkstyle

```
 mvn jxr:jxr checkstyle:checkstyle
```

Suorittaa tiedostoon [checkstyle.xml](https://github.com/JakeKallioniemi/ot-harjoitustyo/blob/master/BrickBreaker/checkstyle.xml) määritellyt tarkastukset. Tuloksia voi tarkastella avaamalla tiedoston _target/site/checkstyle.html_ selaimella.
