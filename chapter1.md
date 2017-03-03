---
title       : Sissejuhatus R-i
description : Siin saab tutvuda tarkvaraga R ja teha esimesi samme programmeerimises :) Alustame!



--- type:NormalExercise lang:r xp:100 skills:1 key:ca824b1118
## R kui kalkulaator

R-i võib kasutada kui kalkulaatorit. Toome ära mõned tehtemärgid:

- Liitmine: +



<!--The ^ operator raises the number to its left to the power of the number to its right: for example 3^2 is 9.
The modulo returns the remainder of the division of the number to the left by the number on its right, for example 5 modulo 3 or 5 %% 3 is 2.
With this knowledge, follow the instructions below to complete the exercise.-->

*** =instructions

Juhised: pead tegema nii ja naa..

*** =hint

Vihjeks nii palju, et ....

*** =pre_exercise_code
```{r}
#polegi
```

*** =sample_code
```{r}
# Calculate 3 + 4
3 + 4

# Calculate 6 + 12
```

*** =solution
```{r}
# Calculate 3 + 4
3 + 4

# Calculate 6 + 12
6 + 12
```

*** =sct
```{r}
test_output_contains("18", incorrect_msg = "Make sure to add `6 + 12` on a new line. Do not start the line with a `#`, otherwise your R code is not executed!")
success_msg("Awesome! See how the console shows the result of the R code you submitted? Now that you're familiar with the interface, let's get down to R business!")
```
