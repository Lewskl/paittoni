---
title: Muuttujat
---

# Muuttujat

Ohjelmoinnissa käsitellään käytännössä aina joitain arvoja, kuten esimerkiksi lukuja tai listoja. Muuttujat ovat yksinkertaisesti sanottuna nimiä, jotka viittaavat arvoihin ja joita voi käyttää arvojen tilalla muualla ohjelmassa.

Pythonissa, kuten monissa muissakin ohjelmointikielissä, muuttuja luodaan eli alustetaan yhtäsuuruusmerkillä =. Esimerkiksi seuraavalla tavalla luodaan muuttuja x, jonka arvo on 7:

    x = 7

Muuttujan nimi on siis ennen yhtäsuuruusmerkkiä, ja arvo sen jälkeen.

Muuttujalle kannattaa valita selkeä nimi, joka kuvaa muuttujan tarkoitusta. Nimi voi sisältää kirjaimia, numeroita ja tiettyjä erikoismerkkejä, mutta nimen ensimmäisen merkin on oltava kirjain tai alaviiva. Ääkköset on tapana korvata varmuuden vuoksi a:lla tai o:lla. Välilyöntejä nimissä ei voi käyttää, joten monisanaisissa nimissä sanat on hyvä erottaa alaviivoilla. Python myös erottaa isot kirjaimet pienistä, joten esimerkiksi `koira` ja `Koira` ovat kaksi erillistä nimeä. Muuttujien nimissä on yksinkertaisuuden vuoksi tapana käyttää ainoastaan pieniä kirjaimia. Tiettyjä sanoja ei myöskään voi käyttää muuttujien niminä, koska niillä on Pythonissa jokin muu toiminto.

Näiden sääntöjen mukaan esimerkiksi `koirien_maara` on parempi nimi kuin `KoirienMäärä`.

Nimen mukaisesti muuttujan arvoa voi muuttaa. Muuttaminen tapahtuu samalla tavalla kuin alustaminenkin.

    x = 19
    x = "koira"
    x = None

[Yleisimmät tietotyypit](../tietotyypit/)