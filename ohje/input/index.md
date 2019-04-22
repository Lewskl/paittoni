---
title: Syötteiden ottaminen
---

# 5. Syötteiden ottaminen

Monet ohjelmat perustuvat käyttäjän antaman tiedon käsittelemiseen. Pythonissa käyttäjän syötteitä otetaan `input()`-funktiolla. Funktio tulostaa sulkujen sisällä annetun merkkijonon ja pysäyttää sitten ohjelman suorituksen kunnes käyttäjä painaa enteriä. Funktio palauttaa käyttäjän syöttämän merkkijonon, joka voidaan esimerkiksi tallentaa muuttujaan.

    nimi = input("Syötä nimesi: ")
    print("Nimesi on siis", nimi)

Funktio palauttaa aina merkkijonon, joten jos syötettä halutaan käyttää esimerkiksi laskutoimituksissa, se pitää muuttaa kokonais- tai liukuluvuksi. Kokonaisluku (englanniksi integer) saadaan `int()`-funktiolla, kun taas liukuluku (englanniksi float) saadaan `float()`-funktiolla.

    x = int(input("Syötä kokonaisluku: "))
    y = float(input("Syötä mikä tahansa luku: "))

Liukuluvuksi kelpaa mikä tahansa luku, kun taas kokonaisluvuksi kelpaa vain kokonaisluku. Jos käyttäjä antaa vääränlaisen syötteen, ohjelma antaa virheilmoituksen ja saattaa lakata toimimasta.

[Ehtolauseet](../ehtolauseet/)