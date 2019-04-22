---
title: Toistorakenteet
---

# 7. Toistorakenteet

Ohjelmoinnissa on monesti hyödyllistä tehdä lähes sama asia monta kertaa peräkkäin. Tätä varten on kehitetty toistorakenteet eli silmukat `while` ja `for`.

## while

`while`-rakenteen syntaksi on samanlainen kuin ehtolauseissa; avainsana `if` vain korvataan avainsanalla `while`. Ehtolauseista poiketen `while`-silmukassa tehtävää asiaa kuitenkin toistetaan niin kauan kunnes ehto lakkaa olemasta tosi. Yleensä on siis järkevää muuttaa jotakin ehdossa käytettyä muuttujaa silmukan sisällä niin, että silmukka loppuu joskus. Jos kuitenkin haluat loputtoman silmukan, voit käyttää ehtoa joka on aina tosi, esimerkiksi `while True:`.

Seuraava esimerkki tulostaa numerot yhdestä kymmeneen:

    x = 1
    while x <= 10:
        print(x)
        x += 1

## for

`for`-silmukka on hieman erilainen: siinä alustetaan silmukan aloittamisen yhteydessä muuttuja, jonka arvo muuttuu silmukan jokaisella suorituskerralla eli iteraatiolla automaattisesti. Yleinen tapa tehdä jokin asia tietty määrä kertoja on käyttää `for`-silmukassa `range()`-funktiota. Funktio luo eräänlaisen listan, jossa on kaikki funktiolle annettujen kokonaislukujen välissä olevat kokonaisluvut. Funktiolle annettu alaraja kuuluu listaan, mutta yläraja ei. Jos funktiolle antaa vain yhden luvun, lista alkaa nollasta.

Jos siis haluat vain tehdä jonkin asian monta kertaa peräkkäin, voit antaa `range()`-funktiolle vain kertojen määrän. Seuraava esimerkki tulostaa sanan "moi" kymmenen kertaa. Esimerkissä i on muuttuja, joka saa vuorotellen jokaisen `range()`-funktion antamista arvoista.

    for i in range(10):
        print("moi")

Jos sen sijaan haluat tehdä numeroilla jotain, anna `range()`-funktiolle suurimmasta haluamastasi luvusta seuraava. Jos et lisäksi halua aloittaa nollasta, joudut antamaan funktiolle myös alarajan. Seuraava esimerkki tulostaa numerot yhdestä kymmeneen yksinkertaisemmin kuin `while`-silmukka.

    for i in range(1, 11):
        print(i)

## break ja continue

Avainsana `break` silmukan sisällä nimensä mukaisesti rikkoo silmukan, jolloin ohjelma jatkaa silmukan jälkeiseen koodiin. Avainsana `continue` sen sijaan lopettaa vain silmukan senhetkisen iteraation, ja ohjelma jatkaa silmukan toistamista. Nämä avainsanat kannattaa laittaa ehtolauseen alle, sillä muuten ne aktivoituvat aina ja niiden merkitys katoaa.