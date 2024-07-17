# Problem 2

In the Middle Ages, one of the problems that required sophisticated algorithmic thinking was determining the date of Easter, which falls on the first Sunday after the first full moon following the vernal equinox. Given this definition, the calculation involves interacting cycles of the day of the week, the orbit of the moon, and the passage of the sun through the zodiac. Early algorithms for solving this problem date back to the third century and are described in the writing of the eight-century scholar known as the Venerable Bede. In 1800, the German mathematician Carl Friedrich Gauss publish an algorithm for determining the date of Easter that was purely computational in the sense that it relied on arithmetic rather than looking up values in tables. His algorithm appears below:

1. Divide the number of the year for which one wishes to calculate Easter by 19, by 4, and by 7, and call the remainders of these divisions `a`, `b`, and `c`, respectively.
2. Divide the value $19a + 24$[^1] by 30 and call the remainder `d`.
3. Divide $2b + 4c + 6d + 5$[^1] by 7 and call the remainder `e`.
4. If $d+e$ is less than 10, then Easter is on March 22 + d + e, otherwise it is on April d + e - 9

[^1]: The last digit of these expressions depends on the century in question. These values are correct for 2000--2099.

Here your task is to write a Python function `find_easter_date` which takes the desired year as an argument and returns a string showing the date of Easter in the specified year. For example, calling `find_easter_date(2020)` should return the string `"April 12"`.

Never assume that your program works properly just because it didn't return an error! The dates of Easter for a handful of years are shown in the table below. Test all of them in your program to make sure they work!

| Year | Easter Date |
|------|-------------|
| 2020 | April 12    |
| 2021 | April 4     |
| 2022 | April 17    |
| 2023 | April 9     |
| 2024 | March 31    |
| 2025 | April 30    |
