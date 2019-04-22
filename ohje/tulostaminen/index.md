---
title: Tekstin tulostaminen
---

# 4. Tekstin tulostaminen

Kuten alkukappaleessa todettiin, Pythonissa tekstiä tulostetaan `print()`-funktiolla. Tulostettavat asiat kirjoitetaan sulkeiden väliin pilkuilla erotettuna, jolloin niiden väliin tulee automaattisesti välilyönti.

    >>> x = 5
    >>> y = 7
    >>> print("x + y =", x+y)
    x + y = 12

`print()`-funktio laittaa tavallisesti tulosteen loppuun rivinvaihdon, mutta jos haluat tulostaa monella funktiolla tekstiä samalle riville, voit antaa funktiolle `end`-parametrin.

    print("tämä teksti on", end=" ")
    print("yhdellä rivillä")

[Syötteiden ottaminen](../input/)