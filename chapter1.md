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

```

*** =sct
```{r}
test_object(c("y", "z"))
test_output_contains("z")
test_error()
success_msg("Great job!")
```









--- type:NormalExercise lang:r xp:100 skills:1 key:b7b1307367
## See on copy-paste näide kogu täiega (https://github.com/datacamp/testwhat/wiki/Quickstart_Guide)


 In this exercise, you'll be calculating a mean.

*** =instructions
- Create a variable `m`, equal to the mean of the numbers 0 up to 9.
- Print out `m`.

*** =hint
- You can use `mean(0:9)` to calculate `m`.
- To print out a variable, simply write the variable name on a new line.

*** =pre_exercise_code
```{r}
# no pre exercise code required
```

*** =sample_code
```{r}
# Calculate the mean of all single digit numbers and assign the result to 'm'



```

*** =solution
```{r}
# Calculate the mean of all single digit numbers and assign the result to 'm'
m <- mean(0:9)
m
```

*** =sct
```{r}
test_correct({
  test_object("m")
}, {
  test_function("mean", args = "x")
})

test_output_contains("m")
test_error()
success_msg("Great job!")

```
    