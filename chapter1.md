---
title       : Sissejuhatus R-i
description : Siin saab tutvuda tarkvaraga R ja teha esimesi samme programmeerimises :) Alustame!



--- type:NormalExercise lang:r xp:100 skills:1 key:ca824b1118
## R kui kalkulaator

R-i võib kasutada kui kalkulaatorit. Toome ära mõned tehtemärgid:

- Liitmine: `+`
- Lahutamine: `-`
- Korrutamine: `*`
- Jagamine: `/`
- Astendamine: `^` või `**`
- Jääk jagamisel: `%%`

ja paar funktsiooni:

- Siinus: `sin()`
- Naturaallogaritm: `log()`
- Kümnenlogaritm: `log10()`


<!--The ^ operator raises the number to its left to the power of the number to its right: for example 3^2 is 9.
The modulo returns the remainder of the division of the number to the left by the number on its right, for example 5 modulo 3 or 5 %% 3 is 2.
With this knowledge, follow the instructions below to complete the exercise.-->

*** =instructions

- Tee läbi Näited 1 kuni 4, ühe rea täitmiseks R script-is vajuta `Ctrl + Enter`.
- Pane tähele, et sümbol  `#` on kasutatud kommentaaride ridade eristamiseks.
- Kirjuta Ülesandesse tehe, mis leiaks $$5^2 + \frac{27}{(4+5)}$$ ja vajuta 'Submit Answer'.

*** =hint

Kui sul tekkisid probleemid märgi `^` leidmisega, siis kasuta selle asemel `**`. Pane tähele, et tehte kirjapanekul on oluline jälgida tehete järjekorda.

*** =pre_exercise_code
```{r}
#polegi
```

*** =sample_code
```{r}
# Näide 1. Liitmine. 
3 + 4

# Näide 2. Jagamine.
8 / 2

# Näide 3. Funktsiooni kasutamine.
sin(2*pi)

# Näide 4. Pikem avaldis.
7 * (8 + 9) - 10 / 5

#Ülesanne


```

*** =solution
```{r}
# Näide 1. Liitmine. 
3 + 4

# Näide 2. Jagamine.
8 / 2

# Näide 3. Funktsiooni kasutamine.
sin(2*pi)

# Näide 4. Pikem avaldis.
7 * (8 + 9) - 10 / 5

#Ülesanne
5^2 + 27 / (4 + 5)

```

*** =sct
```{r}
test_output_contains("5^2 + 27 / (4 + 5)", incorrect_msg = "Viga1")
success_msg("Tubli! Suundu järgmise ülesande juurde.")
```

<--! Järmine harjutus-->


--- type:NormalExercise lang:r xp:100 skills:1 key:3b528fab71
## Muutujad

Ka kalkulaatorit kasutades tekib peatselt vajadus meeles pidada arvutuste tulemusi. R-is võivad muutujate nimed sisaldada suuri ja väikesi tähti, numbreid; punkti ja alakriipsu. Erandiks on see, et nimi ei või alata numbri või alakriipsuga. Näiteks saab omistada `x`-le väärtuse 3 järgmiselt: `x <- 3`. 


*** =instructions

- Proovi läbi näitekood.
- Ülesanne: omista muutujale `z` summa, mille liidetavad on `y` ja 5. Väljasta `z` väärtus ekraanile.
- Ülesanne vastuse kontrolli paika saamiseks. Sisesta käsud
    * `vec <- 0:9`
    * `m <- sum(vec)/length(vec)`
    * `m`

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Näide 1. Omistame muutjale y väärtuse 2 ja väljastame väärtuse
y <- 2
y

# Näide 2. Kasutame muutujat y arvutuses
y + 5

# Ülesanne
z <- y + 5
z

# Näide DataCampist ülesande kontrolli tegemiseks


```

*** =solution
```{r}
# Näide 1. Omistame muutjale y väärtuse 2 ja väljastame väärtuse
y <- 2
y

# Näide 2. Kasutame muutujat y arvutuses
y + 5

# Ülesanne
z <- y + 5
z

# Näide DataCampist ülesande kontrolli tegemiseks
vec <- 0:9
m <- sum(vec)/length(vec)
m
```

*** =sct
```{r}
test_correct({
  test_object("z")
}, {
  test_function("+")
})

test_output_contains("z")
test_error()
success_msg("Great job!")
```








