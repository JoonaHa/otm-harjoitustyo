# OTM-harjoitustyö

Harjoitustyön, sekä viikottaisten tehtävien, *repo* **ohjelmistotekniikan mekaniikat** -kurssia varten.

Yksinkertainen ylhäältäpäin kuvattu räiskintäpeli, jossa pelaajan pitää puolustaa itseään pimeydessä, apunaan hänen luotettava taskulamppunsa.

## Dokumentaatio
* [Testausdokumentti](https://github.com/JoonaHa/OTM-harjoitustyo/blob/master/dokumentaatio/testaus.md)
* [Käyttöohje](https://github.com/JoonaHa/OTM-harjoitustyo/blob/master/dokumentaatio/kayttoohje.md)
* [Vaatimusmaarittely](https://github.com/JoonaHa/OTM-harjoitustyo/blob/master/dokumentaatio/vaatimusmaarittely.md)
* [Arkkitehtuurikuvaus](https://github.com/JoonaHa/OTM-harjoitustyo/blob/master/dokumentaatio/arkkitehtuuri.md)
* [Tuntikirjanpito](https://github.com/JoonaHa/OTM-harjoitustyo/blob/master/dokumentaatio/tuntikirjanpito.md)
## Releaset
* [Loppupalautus](https://github.com/JoonaHa/OTM-harjoitustyo/releases/tag/v1.0)
* [Viikko 6](https://github.com/JoonaHa/OTM-harjoitustyo/releases/tag/v.06.1)
* [Viikko 5](https://github.com/JoonaHa/OTM-harjoitustyo/releases/tag/v0.5)
## Komentorivitoiminot
* **Huom!** Muista siirtyä oikeaan kansioon ennen komentojen suorittamista. Esimerkiksi:
```
cd PitchBlack/
```

Ohjelman **JUnit-testit** voi suorittaa komennolla:
```
mvn test
```

Testeistä voi luoda **kattavuusraportin** komennolla:
```
mvn jacoco:report
```
Raportti on html-dokumentti _target/site/jacoco/index.html_ jota voi tarkastella selaimella. 


Ohjelmasta voi luoda **jar-paketin** komennolla:
```
mvn package
```
Suoritettava tiedosto löytyy _target_-hakemistosta nimellä _target/OtmPitchBlack-1.0-SNAPSHOT.jar_

**Checkstyle** tarkistukset suoritetaan komennolla.Tarkistuksen määritykset ovat [checkstyle.xml](https://github.com/JoonaHa/OTM-harjoitustyo/commit/7c27f14ffdb24160d2a4caa23cc9638d1af4f51f) tiedostossa.
```
 mvn jxr:jxr checkstyle:checkstyle
```
Tarkistuksen tulokset löytyvät _target/site/checkstyle.html_ tiedostosta.

**JavaDoc** pystyy generoimaan komennolla:

```
mvn javadoc:javadoc
```

JavaDocia voi tarkastella selaimella tiedostosta _target/site/apidocs/index.html_


