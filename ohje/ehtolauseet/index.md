---
title: Ehtolauseet
---

# 6. Ehtolauseet

Ehtolauseiden avulla ohjelma voi päättää saamansa tiedon perusteella mitä tehdä seuraavaksi. Ehtolauseen yksinkertaistettu muoto on "jos ehto on tosi, niin tee asia x". Pythonissa ehtolauseen alussa on avainsana `if` ja ehdon jälkeen kaksoispiste. Tehtävä asia sisennetään joko neljällä välilyönnillä tai Q-näppäimen vasemmalla puolella olevalla sarkaimella, jotta tietokone erottaa sen ohjelman muista osista.

    if ehto:
        print("ehto on tosi")

Ehdoissa käytetään matematiikasta tuttuja vertailumerkkejä:

- "<" - pienempi kuin

- ">" - suurempi kuin

- "==" - yhtä suuri kuin

- "!=" - erisuuri kuin

- "<=" - pienempi tai yhtä suuri kuin

- ">=" - suurempi tai yhtä suuri kuin

Esimerkiksi seuraava ehtolause toteutuu vain silloin, kun x on negatiivinen:

    if x < 0:
        print("x on negatiivinen")

Ehtolauseeseen voi lisätä myös asian, joka tehdään siinä tapauksessa että ehto ei toteudu. Tämä tehdään `else`-avainsanalla ("muuten").

    if x < 0:
        print("x on negatiivinen")
    else:
        print("x ei ole negatiivinen")

Lisäksi samaan sarjaan voi lisätä useampia ehtolauseita, joita kokeillaan jos edellinen ehto ei toteudu. Tähän käytetään avainsanaa `elif`, joka on avainsanojen `else` ja `if` yhdistelmä. `else` on aina viimeisenä.

    if x < 0:
        print("x on negatiivinen")
    elif x > 0:
        print("x on positiivinen")
    else:
        print("x on nolla")

## Totuusarvot ehtolauseissa

Kaikki vertailut palauttavat joko True tai False riippuen siitä, onko vertailu tosi vai epätosi.

    >>> 2 < 5
    True
    >>> 0 == 100
    False

Ehtolause toteutuu, jos ehto palauttaa arvon `True`. Koska totuusarvomuuttujien arvo on aina vain joko `True` tai `False`, niitä voi käyttää ehtolauseissa sellaisenaan.

    if x:
        print("x on tosi")

Operaattori `not` vaihtaa totuusarvon päinvastaiseksi.

    >>> not True
    False
    >>> not False
    True

Sen avulla voi tehdä ehtolauseen, joka toteutuu kun totuusarvomuuttuja on epätosi.

    if not x:
        print("x on epätosi")

## Listojen tarkastaminen

Operaattorilla `in` on helppo tarkistaa kuuluuko arvo listaan.

    lemmikit = ["kissa", "koira", "kani", "käärme"]
    elain = input("Anna eläin: ")
    if elain in lemmikit:
        print("Eläimesi on lemmikkieläin!")

Listojen käsittelyssä voi hyödyntää myös `not`-operaattoria.

    if elain not in lemmikit:
        print("Antamasi eläin ei sovi lemmikiksi.")

`in`-operaattorilla voi etsiä myös merkkijonojen osia ja sanakirjojen avaimia.

    >>> lause = "En ole käynyt Espanjassa."
    >>> "nyt" in lause
    True

    >>> auto = {"merkki": "Audi", "vari": "valkoinen"}
    >>> "merkki" in auto
    True

## Ehtojen yhdistäminen

Joissain tilanteissa samaan ehtolauseeseen on järkevää yhdistää useita ehtoja. Tämä tehdään operaattoreilla `and` ja `or`. Ehto jossa on `and` toteutuu vain jos operaattorin molemmilla puolilla olevat ehdot toteutuvat, kun taas ehdossa jossa on `or` riittää että toinen ehdoista toteutuu.

    if x > 10 and x < 20:
        print("x on yli 10 ja alle 20")

    if lemmikki == "kissa" or lemmikki == "koira":
        print("lemmikki on kissa tai koira")

Jos ehdossa käytetään molempia operaattoreita, ehtoa kannattaa selkeyttää sulkeilla.

    if (x < -10 or x > 10) and x % 3 == 0:
        print(x**2)

[Toistorakenteet](../toistorakenteet/)