# porcelainporcupines

Installation
------------

``` r
devtools::install_github("abern041/porcelainporcupines")
```

Usage
-----

``` r
library("porcelainporcupines")
```

View all palette names
``` r
names(porcelain_porcupines)
[1] "GA1"       "ZABA"      "HTBAHB"    "Dreamland" "WarmGlow"  "Landmark" 
[7] "Bambi"     "LP3"       "Loser"
```

Palettes
--------

### Glass Animals

``` r
porcelain_porcupine("Dreamland")
```

![Dreamland](https://user-images.githubusercontent.com/55102014/165415576-a9a37ca5-c2c4-4c7f-86d7-f110d92aeffb.jpg)

``` r
porcelain_porcupine("HTBAHB")
```

![HTBAHB](https://user-images.githubusercontent.com/55102014/165415735-c757f2aa-9099-48c4-ae20-e4b0e7adf17b.jpg)

``` r
porcelain_porcupine("ZABA")
```

![ZABA](https://user-images.githubusercontent.com/55102014/165415785-3b99c591-cf17-4b76-96db-e8dad4a671c1.jpg)

``` r
porcelain_porcupine("GA1")
```

![GA1](https://user-images.githubusercontent.com/55102014/165415841-317155d1-281f-4e96-b85e-be1286d82698.jpg)

### Hippo Campus

``` r
porcelain_porcupine("WarmGlow")
```

![WarmGlow](https://user-images.githubusercontent.com/55102014/165415900-634776c8-ae43-4693-af08-a632df1a6cef.jpg)

``` r
porcelain_porcupine("Landmark")
```

![Landmark](https://user-images.githubusercontent.com/55102014/165416079-8efd28a4-1f39-4746-8f08-42652e58c950.jpg)

``` r
porcelain_porcupine("Bambi")
```

![Bambi](https://user-images.githubusercontent.com/55102014/165416022-6f2aae06-aa73-44f9-b1f6-717494815ae6.jpg)

``` r
porcelain_porcupine("LP3")
```

![LP3](https://user-images.githubusercontent.com/55102014/165416122-886dcf04-cbf3-42fd-a17b-a5f5ac8ee5dd.jpg)

``` r
porcelain_porcupine("Loser")
```

### Loser Magnet

![Loser](https://user-images.githubusercontent.com/55102014/165416183-b93daa98-6024-41a8-9db6-2567456b1472.jpg)


Examples of use
-----

``` r
ggplot(mpg, aes(displ, hwy, colour = class)) + 
+     geom_point() + scale_color_manual(values = porcelain_porcupine("GA1")) + theme_bw()
```

![mtcars_GA1](https://user-images.githubusercontent.com/55102014/170151988-afec9def-27b9-42ca-b2da-84d70386ffb6.jpg)

``` r
df2 <- data.frame(supp=rep(c("VC", "OJ"), each=3),
                  dose=rep(c("D0.5", "D1", "D2"),2),
                  len=c(6.8, 15, 33, 4.2, 10, 29.5))
ggplot(data=df2, aes(x=dose, y=len, fill=supp)) +
  geom_bar(stat="identity") + scale_fill_manual(values = porcelain_porcupine("LP3")) + theme_bw()
```
![juice_LP3](https://user-images.githubusercontent.com/55102014/170153047-0221f1c8-bc8d-4c37-8282-f323ee57134f.jpg)


