---
title: Matematiikka
---

# 3. Matematiikka

Kaikenlainen matematiikka on olennainen osa ohjelmointia. Peruslaskutoimitukset toimivat aivan samalla tavalla kuin muuallakin, mutta on hyvä tietää, että tietokoneympäristössä kertomerkki on "\*" ja jakomerkki "/". Lisäksi Pythonissa potenssimerkki on "\*\*"; esimerkiksi `3 ** 2` on 9. Kaikenlaisia laskutoimituksia voi tehdä käytännössä kaikkialla, sillä laskutoimituksen tulos on yksittäinen arvo. Laskujärjestys on tietysti sama kuin aina matematiikassa.

    x = 3
    y = x * 4
    z = (y - 2) * x

## Jakojäännös

Koulumatematiikassa jakojäännökset jäävät pois melkein heti jakolaskun opettelemisen jälkeen, mutta ohjelmoinnissa ne ovat tärkeitä. Kertauksena: jakojäännös on se mitä jakolaskussa jää jäljelle, kun jako ei mene tasan. Esimerkiksi jakolaskun 10 / 4 jakojäännös on 2. Jakojäännösmerkki eli modulus on ohjelmoinnissa käytännössä aina prosenttimerkki "%".

Edellisen esimerkin jakojäännös saadaan Pythonissa siis laskutoimituksella `10 % 4`.

Jakojäännöksellä voi esimerkiksi tarkistaa, onko jokin luku jaollinen jollain toisella luvulla; jos jako menee tasan, jakojäännös on nolla. Tällä tavalla voi myös tarkistaa onko luku parillinen vai pariton, koska kaikki parilliset luvut ovat jaollisia kahdella.

## Lattiajako

Jos jako ei mene tasan ja jaettava on kokonaisluku, Python muuttaa sen automaattisesti liukuluvuksi. Jos kuitenkin esimerkiksi halutaan tietää montako kertaa 4 menee kokonaisena lukuun 10, pitää käyttää lattiajakoa, jonka merkki on "//". Lattiajaossa tulos käytännössä pyöristyy alaspäin; esimerkiksi `10 / 4` on 2.5, mutta `10 // 4` on vain 2.

## Muuttujien muokkaaminen

Muuttujien arvoja on monesti hyödyllistä muokata matemaattisesti. Esimerkiksi seuraava rivi kasvattaa muuttujan x arvoa viidellä:

    x = x + 5

Tälle on kuitenkin helpompi merkintätapa:

    x += 5

Matemaattinen operaattori ennen yhtäsuuruusmerkkiä tarkoittaa, että muuttujan arvolla tehdään jokin laskutoimitus, ja tuloksesta tulee muuttujan uusi arvo.

    x = 8
    x /= 2

Muuttuja x siis jaettiin kahdella, eli sen uusi arvo on neljä.

## Merkkijonojen käsittely

Merkkijonoja voi yhdistää plusmerkillä ja monistaa kertomerkillä.

    >>> "yhdys" + "sana"
    'yhdyssana'
    >>> "koira" * 3
    'koirakoirakoira'

[Tekstin tulostaminen](../tulostaminen/)