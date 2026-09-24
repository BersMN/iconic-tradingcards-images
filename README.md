# iconic-tradingcards-images

Card artwork for `resources/[custom]/iconic-tradingcards` on the iconic server.

```
cards/a/    A rank   (80% of pack pulls)
cards/s/    S rank   (15%)
cards/sp/   S+ rank  ( 5%)  - currently all the same "PICK AGAIN" placeholder,
                             replace a file to give that card its own art
cards/backcard.png   face-down card back
```

The `iconic_tradingcards` table points at these files:

    https://raw.githubusercontent.com/BersMN/iconic-tradingcards-images/main/cards/a/Comiccard_A_2B.png

Replacing a picture = commit the new file under the same name. The next pack /
card use shows it (no SQL, no restart). A brand new card needs a row in the
table and an item in `qb-core/shared/items.lua`.
