# iconic-tradingcards-images

Card artwork for `resources/[custom]/iconic-tradingcards` on the iconic server.

```
cards/a/      A rank cards    70   (80% of a Mystery Card pull)
cards/s/      S rank cards    49   (15%)
cards/sp/     S+ rank cards   31   ( 5%)  - all the same "PICK AGAIN" placeholder
                                            for now, replace a file to give that
                                            card its own art
figures/a/    A rank figures  31   (80% of a Mystery Box pull)
figures/s/    S rank figures  25   (15%)
figures/sp/   S+ rank figures 17   ( 5%)
packs/        the two pack items (Mystery Box / Mystery Card)
cards/backcard.png   face-down card back
```

The `iconic_tradingcards` table points at these files:

    https://raw.githubusercontent.com/BersMN/iconic-tradingcards-images/main/cards/a/Comiccard_A_2B.png

Replacing a picture = commit the new file under the same name. The next pack /
card use shows it (no SQL, no restart). A brand new card needs a row in the
table and an item in `qb-core/shared/items.lua`.
