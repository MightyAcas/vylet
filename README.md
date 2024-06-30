# Vylet

```
  w c m p b  x l o u j -
  r s t h f  y n a e i ,
  q v g d k  z * ' ; .  
```

i think its easiest just to show you a list of the most common SFBs in this layout:

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

all of the top 8 sfbs are addressed, either in part or in full, by one of the following techniques:
- alt fingering
- slides
- magic key

I thought about explaining what those are, but honestly if you're reading this you already know what those are. And if not, go read Ec0vid's layout doc.

## Alt Fingering

Alt fingering on a colstag keyboard is typically less preferred than rowstag, but there's still room to make it work. Namely with where I've placed my `L` and `Y` keys. The major bigrams created from this position is `LY`. Using the Monkeyracer corpus shows this bigram creates 0.38% SFBs.

I should meantion that these alt fingers don't outright erase the total SFB percentage here. Because they involve the middle finger, any word that uses a letter on the right hand middle finger (`O` or `A`), followed by `LY` is still a SFB. so words like `holy` or `really` contain SFBs.

ly    0.377%

Examples of ly in MONKEYRACER:
5,050 / 406,279 words (1.243%)

Examples of [ao]ly in MONKEYRACER:
71 / 406,279 words (0.017%)

analysis          (12)
holy              (12)
melancholy         (8)
italy              (5)
analyzing          (4)
analyze            (4)
paralyzed          (4)
apocalypse         (3)
analytic           (3)
olympic            (2)

Examples of lly in MONKEYRACER:
1,282 / 406,279 words (0.316%)

Examples of [ao]lly in MONKEYRACER:
1,153 / 406,279 words (0.284%)

really           (400)
actually         (119)
finally           (81)
usually           (70)
especially        (41)
eventually        (35)
literally         (21)
naturally         (21)
totally           (19)
generally         (19)

the `LY` alt finger does not eliminate the full 0.377% SFBs that `LY`; It instead covers 0.286% SFBS. This means 0.091% SFBs is the true amount of SFBs `LY puts on the Vylet layout.

these calculations were done by hand so there's always a chance i made a mistake, or i'm just plain missing something. just something to be aware of in case you were wondering.

`NY` is also in a good spot to be alt fingered. I had originally designed this layout with it in mind, but over time I've opted against it. 

It's worth noting that this alt fingering wouldn't work as well if the chosen bigrams tend to reverse direction. In my case, instances of `YL` and `YN` are rather rare, which means learning the alt fingers and integrating them into your typing happens rather quickly. The irony of `vylet` having `yl` in the name is not lost on me.

### NL

ok this bigram is a bit deceiving.

```
Examples of nl in MONKEYRACER:
1,176 / 406,279 words (0.289%)

only             (892)
suddenly          (84)
unless            (50)
certainly         (24)
sunlight          (14)
unlike            (14)
moonlight         (14)
commonly           (7)
online             (7)
unlikely           (6)
```
Out of the 1,176 instances of `nl` in the corpus, 892 of them are from `only` (76% of all `nl` instances). and in vylet, the `nl` bigram in `only` gets split up by typing `on` as normal and then alt fingering `ly`. I thought this would be slow but I'm consistently able to get burst speeds over 100wpm with this particular word. so at least for this bigram, I'm realistically only dealing with a quarter of the `nl` SFBs (which would be 0.021%).

## Slides

`OA`, `UE`, and `PH` are all comfortable downwards slides for me. `NY` is also a slide, just a sideways one.

## Magic Key

This leaves me with two bigrams to address: `SC` and `WR`. I could slide `SC`, but upwards slides are much less comfortable than their downwards counterpart. `WR` is downwards, but is on the pinky which doesn't feel well-suited to do slides at least for my hands. This is why they would ultimately become rules for my magic key.

### Magic Key Rules

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

## Top SFBS revisited

```
Top 10 vylet SFBs:
ly    0.091%
ny    0.000%
ue    0.000%
sc    0.000%
nl    0.021%
oa    0.000%
ph    0.000%
wr    0.000%
e;    0.013%
rw    0.012%
```

fyi i'm treating this like a blog and less like a concise description of my layout. like i'll talk about specifics with my layout but also wanna go into what got me there in the first place. enjoy the ride :D

## Background
Vylet is the product of my ongoing keyboard layout hyperfixation, which started almost 2 years ago from now (6/29/24). I stumbled on the [r/keyboardlayouts subreddit](https://www.reddit.com/r/KeyboardLayouts/), which led to me learning a few different alternative keyboard layouts over the course of a year and a half. By mid-December 2023, I started creating my own layouts and would tweak a letter's position every couple of days based on my comfort with it. I did this over the course of 2 months, and by February I had the first concrete version of Vylet: 

```
  w c m p k  q l o u j -
  r s t h f  y n a e i ,
  z v g d b  x * ' / .  
```

Cool! It's still a few swaps off from being the current version, but it's close enough where I wouldn't consider it outright different.

## Motivation

I won't bullshit you, I didn't care about stats

![image](https://github.com/MightyAcas/Vylet/assets/67846394/6e8ac65a-fb34-4490-8065-b94b6cc715c7)
