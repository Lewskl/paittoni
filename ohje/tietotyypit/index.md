---
title: Yleisimmät tietotyypit
---

# Yleisimmät tietotyypit

## Luvut

Ohjelmoinnissa tarvitaan lähestulkoon aina kokonaislukuja. Tietokoneen näkökulmasta liukuluvut (eli käytännössä desimaaliluvut) ja kokonaisluvut ovat täysin eri asioita, joten on tärkeää muistaa kumpia käsittelee. Laskutoimituksissa Python kuitenkin muuttaa kokonaisluvut tarvittaessa liukuluvuiksi, mikä tekee matematiikasta merkittävästi helpompaa. On hyvä huomata, että liukuluvuissa käytetään desimaalipistettä eikä -pilkkua. Ohjelmissa ei tarvitse erikseen määrittää, että jokin arvo on kokonais- tai liukuluku, vaan tietokone näkee sen itse.

    x = 42
    y = 3.14

## Merkkijonot

Ohjelmissa käytettäviä tekstinpätkiä kutsutaan merkkijonoiksi. Merkkijonot erotetaan muista arvoista siten, että ne rajataan yksin- tai kaksinkertaisilla lainausmerkeillä (' tai "). Selkeyden vuoksi saman ohjelman sisällä kannattaa pyrkiä käyttämään mahdollisimman usein vain yhdenlaisia lainausmerkkejä.

    'suomi'
    "ruotsi"

Jos haluat käyttää merkkijonon sisällä lainaus- tai heittomerkkejä, kannattaa rajata merkkijono eri merkeillä, kuin mitä itse merkkijono sisältää.

    'Sanaa "tahi" käytetään nykyään harvoin.'

Jos merkkijono sisältää sekä lainaus- että heittomerkkejä, voit laittaa rajausmerkkien kanssa konfliktoivien merkkien eteen kenoviivan (\\). Kenoviiva kertoo tietokoneelle, että seuraava merkki ei vaikuta ohjelman toimintaan, vaan on vain osa merkkijonoa.

    "It's called \"fool's gold\" for a reason."
    'It\'s called "fool\'s gold" for a reason.'

## Totuusarvot

Totuusarvot ovat tietotyypeistä ehkä yksinkertaisimpia: niiden arvo voi olla vain tosi (`True`) tai epätosi (`False`). Ne ovat kuitenkin äärettömän hyödyllisiä. Pythonissa arvoilla `True` ja `False` on oltava iso alkukirjain. Totuusarvot eivät vaadi mitään lisämerkkejä, koska `True` ja `False` on varattu käytettäväksi pelkästään totuusarvoissa.

## Listat

Listat ovat hyödyllisiä, jos samaan asiaan liittyviä tietoja halutaan pitää yhdessä paikassa. Listan ympärillä on hakasulkeet, ja sen sisältämät arvot eli alkiot erotetaan toisistaan pilkulla.

    auto = ["Audi", "valkoinen", 2016]

Listan alkioihin viitataan niiden paikkanumeroilla eli indekseillä. On erittäin tärkeää muistaa, että listojen indeksointi alkaa nollasta, eli listan ensimmäinen alkio on indeksissä 0.

    >>> auto[0]
    'Audi'
    >>> auto[1]
    'valkoinen'
    >>> auto[2]
    2016

Alkioiden arvoja voi muuttaa samaan tapaan kuin muuttujia.

    auto[1] = "musta"

Listaan voi lisätä alkioita `append()`-funktiolla. Sulkujen sisällä oleva arvo lisätään listan loppuun.

    auto.append("60000€")

## Sanakirjat

Sanakirjat ovat käytännössä listoja, joiden alkioilla on indeksin sijaan nimi. Nimet voivat olla esimerkiksi lukuja, merkkijonoja tai totuusarvoja. Sanakirjoissa käytetään hakasulkeiden sijaan aaltosulkeita, ja alkioiden nimien ja arvojen väliin tulee kaksoispiste.

    auto = {"merkki": "Audi", "vari": "valkoinen", "vuosi": 2016}

Sanakirjan alkioiden arvoihin viitataan samalla tavalla kuin listan alkioihin.

    >>> auto["merkki"]
    'Audi'
    >>> auto["vari"]
    'valkoinen'
    >>> auto["vuosi"]
    2016

Myös sanakirjan alkioiden arvoja voi muuttaa muuttujien tapaan.

    auto["vari"] = "musta"

Alkioiden lisääminen sanakirjaan ei vaadi erillistä funktiota. Voit yksinkertaisesti määrittää uuden alkion kuin muuttujan.

    auto["hinta"] = "60000€"

[Matematiikka](../matematiikka/)