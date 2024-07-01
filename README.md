# Vylet

<img src="img/vylet_keymap.svg" alt="vylet keymap" width="100%" />

```
  w c m p b  x l o u j -
  r s t h f  y n a e i ,
  q v g d k  z * ' ; .  
```

Vylet is the product of my ongoing keyboard layout hyperfixation, which started about 2 years ago from now. It's been almost 6 months since I started using it. The layout started out as a mod of [Wedlock](https://github.com/GGabi/wedlock) before evolving into its own thing. Vylet takes inspiration from [APTv3](https://github.com/Apsu/APT), [Workman](https://workmanlayout.org/), and [Magic Sturdy](https://github.com/Ikcelaks/keyboard_layouts/blob/main/magic_sturdy/magic_sturdy.md). You may want to click that last link if you don't know what a magic key `*` is, since this layout makes use of it. It also takes advantage of alt fingerings and slides, so I hope you know what those are too. If not, go read Ec0vid's layout doc.

## Goals
By the time I started making my own mods/layouts in December 2023, I had already had a year of experience with [Colemak DH](https://colemakmods.github.io/mod-dh/), a month with [Canary](https://github.com/Apsu/Canary), and a bunch of weeks spread between a couple other layouts. Learning and typing daily with these allowed me to get a better grasp of what I wanted out of a layout. So when setting out to make a layout tailored to me, these were the characteristics I was aiming for:
- Balanced finger use
- High inrolls
- Low scissors (with little to no full scissors)
- Low LSBs
- Low index use, but only on the right hand (most likely strain from mouse clicking)

## Background

When doing my initial modding, I would tweak a letter's position every couple of days based on my comfort with it. I did this over the course of 2 months, and eventually realized I was making something very similar to APTv3. I had originally passed on learning this layout when I heard about it a year ago, but on second look it seemed like it had all the characteristics I was looking for. There was one exception: the letter `Y`.

On APTv3, `Y` is placed on the top row of the right pinky. This would break my rules by introducing some nasty pinky-ring scissor interactions, as well as putting the pinky's usage above what I'd prefer. This is what got me thinking about where to place Y, and deciding to optimize its placement based on alt fingering.

## Alt Fingering

The placement of `Y` in Vylet creates only 2 significant bigrams: `LY` and `NY`. Both of these bigrams can be alt fingered comfortably, which negates most of the SFBs this `Y` placement creates. We're just gonna focus on talking about `LY` since its the far more important SFB, and I tend to slide `NY` instead of alting it anyway.

Keep in mind that alt fingering doesn't just erase the total SFB percentage here (which is 0.377% in Monkeyracer). The `LY` alt finger starts with the middle finger, meaning any word that uses a letter on the right hand middle finger (`O` or `A`), followed by `LY` is still a SFB. This means words like `holy` or `really` contain SFBs in Vylet.

Taking this into account, the SFBs caused by `LY` in this layout isn't 0.377%, but instead is 0.091%.

## Slides

`OA`, `UE`, and `PH` are all comfortable downwards slides for me. `NY` is also a slide, just a sideways one. It's worth mentioning that this technique doesn't work as well if you're on a standard mechanical keyboard with the taller, more spaced out keys. Low profile keyboards with light switches, and especially laptop keyboards are best suited for this.

## Magic Key

This leaves me with two significant SFBs in Vylet to address: `SC` and `WR`. I could slide `SC`, but upwards slides are much less comfortable than their downwards counterpart. `WR` is downwards, but is on the pinky which doesn't feel well-suited to do slides at least for my hands. This is why they would ultimately become rules for my magic key.

### Magic Key Rules

Below is my full set of magic rules used on Vylet.

```
// full scissor bigram (FSB)
c★      ⇒ ck
'★      ⇒ 'l
l★      ⇒ ll

// half scissor bigram (HSB)
g★      ⇒ gh
p★      ⇒ pt
r★      ⇒ rk

// same finger bigram (SFB)
s★      ⇒ sc
w★      ⇒ wr

// lateral stretch bigram (LSB)
f★      ⇒ ft
m★      ⇒ mb

// half scissor LSB
b★      ⇒ bt
a★      ⇒ ax
e★      ⇒ ex
i★      ⇒ ix
```

Most of these should be self-explanatory except the 3 `X` rules at the end. `X` can be annoying on the vowel side because in words, it's often between 2 other vowels (`exist`, `exactly`, `example`, etc.). This means any involvement of `X` in a word is likely going to be a redirect. these 3 rules make the redirects less of an issue since `X` is now in a closer, more comfortable spot.

## Analyzer Stats

### Cyanophage

![image](https://github.com/MightyAcas/Vylet/assets/67846394/b03b6d74-4a62-428f-b645-c9db817e6469)
![image](https://github.com/MightyAcas/Vylet/assets/67846394/5006ad33-4867-4fab-a82e-3adf97f90613)
![image](https://github.com/MightyAcas/Vylet/assets/67846394/0248289c-17d3-4322-87d6-d8bc88500e25)
![image](https://github.com/MightyAcas/Vylet/assets/67846394/10aec98f-fc50-4a6a-8d0e-3cae120545fc)

Here's the [link](https://cyanophage.github.io/playground.html?layout=wcmpbxlouj-rsthfynaei%2Cqvgdkz%2F%27%3B.%5C&mode=ergo) if you want to edit Vylet yourself.

### Keysolve

![image](https://github.com/MightyAcas/Vylet/assets/67846394/1b375c9d-c331-40ae-beb2-f56a53ce92e1)
![image](https://github.com/MightyAcas/Vylet/assets/67846394/f536648a-1d93-41e3-b3d1-1715b47102a5)


### Layout Playground

![image](https://github.com/MightyAcas/Vylet/assets/67846394/68726cb7-74f8-4cfa-9b6b-8d621455da27)

### cmini

```
vylet (acas) (10 likes)
  w c m p b  x l o u j -
  r s t h f  y n a e i ,
  q v g d k  z * ' ; .  

MONKEYRACER:
  Alt: 27.00%
  Rol: 47.40%   (In/Out: 32.99% | 14.42%)
  One:  2.99%   (In/Out:  1.16% |  1.82%)
  Rtl: 50.39%   (In/Out: 34.15% | 16.24%)
  Red:  3.98%   (Bad:     0.26%)

  SFB: 0.93%
  SFS: 6.03%    (Red/Alt: 1.85% | 4.18%)

  LH/RH: 45.22% | 54.78%
```
```
Top 10 vylet SFBs:
ly    0.377%
ny    0.140%
ue    0.099%
sc    0.092%
nl    0.084%
oa    0.045%
ph    0.044%
wr    0.039%
e;    0.013%
rw    0.012%
```
```
Top 10 vylet SFS:
gt    0.547%
wr    0.462%
ue    0.461%
ln    0.388%
ao    0.351%
o'    0.304%
mt    0.253%
tm    0.250%
i.    0.207%
cs    0.184%
```
```
Top 10 vylet Alternates:
hat   0.865%
her   0.635%
ver   0.509%
for   0.449%
ome   0.400%
his   0.362%
ter   0.359%
are   0.341%
ave   0.315%
wit   0.280%
```
```
Top 10 vylet Rolls:
the   2.656%
ing   1.382%
and   1.191%
tha   0.664%
thi   0.598%
hin   0.479%
our   0.443%
ent   0.376%
rea   0.344%
not   0.331%
```
```
Top 10 vylet Inrolls:
the   2.656%
ing   1.382%
and   1.191%
tha   0.664%
thi   0.598%
hin   0.479%
ent   0.376%
rea   0.344%
the   0.311%
ith   0.308%
```
```
Top 10 vylet Onehands:
you   1.166%
ion   0.383%
you   0.182%
eal   0.127%
ien   0.093%
rst   0.083%
ean   0.077%
ou.   0.056%
ual   0.056%
rth   0.053%
```
```
Top 10 vylet Redirects:
one   0.359%
oul   0.249%
ain   0.210%
oun   0.172%
ine   0.161%
str   0.126%
lea   0.126%
oin   0.098%
eli   0.086%
thr   0.084%
```

#### Finger Use
```
vylet (usage) (acas) (10 likes)
  w c m p b  x l o u j -
  r s t h f  y n a e i ,
  q v g d k  z * ' ; .  

MONKEYRACER:
  LI: 13.30%    RI: 14.10%
  LM: 12.52%    RM: 16.11%
  LR:  9.33%    RR: 16.58%
  LP:  8.20%    RP:  9.85%

  Total: 100.00%
```
```
vylet (sfb) (acas) (10 likes)
  w c m p b  x l o u j -
  r s t h f  y n a e i ,
  q v g d k  z * ' ; .  

MONKEYRACER:
  LI:  0.09%    RI:  0.42%
  LM:  0.04%    RM:  0.08%
  LR:  0.11%    RR:  0.13%
  LP:  0.05%    RP:  0.02%

  Total: 0.93%
```
```
vylet (sfs) (acas) (10 likes)
  w c m p b  x l o u j -
  r s t h f  y n a e i ,
  q v g d k  z * ' ; .  

MONKEYRACER:
  LI:  0.81%    RI:  0.93%
  LM:  1.20%    RM:  1.00%
  LR:  0.53%    RR:  0.66%
  LP:  0.57%    RP:  0.41%

  Total: 6.11%
```
```
vylet (acas) (10 likes)
MONKEYRACER:
Unweighted Speed
    LP: 2.812
    LR: 3.784
    LM: 6.448
    LI: 8.107
    RI: 17.668
    RM: 8.545
    RR: 3.801
    RP: 2.418

Weighted Speed
    LP: 1.874
    LR: 1.051
    LM: 1.343
    LI: 1.474
    RI: 3.212
    RM: 1.780
    RR: 1.056
    RP: 1.612
```

## Credits
[Cyanophage](https://cyanophage.github.io/index.html), [Pine](https://clemenpine.github.io/keysolve-web/), and [Oxey](https://oxey.dev/playground/index.html) for their web-based keyboard layout analyzers. Their ease of access has been invalable for me.
