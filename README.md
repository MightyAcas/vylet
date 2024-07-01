# Vylet

<img src="img/vylet_keymap.svg" alt="vylet keymap" width="100%" />

```
  w c m p b  x l o u j -
  r s t h f  y n a e i ,
  q v g d k  z * ' ; .  
```
`*/★` = magic key

# Introduction

Vylet is a keyboard layout I made over the course of two months with the help of online layout analyzers like [Cyanophage](https://cyanophage.github.io/index.html). These kinds of sites allow you to manually move around letters and see the resulting stats, which was how my layout was created. I've been using Vylet for almost six months now and just recently reached 100wpm with it. I have no intentions of switching from it any time soon, and plan to ride it into the sunset. I'll this writeup once I hit one year with it!

![image](https://github.com/MightyAcas/Vylet/assets/67846394/fd36a2c0-2ba6-4e25-8d3b-95467f16de06)

This layout is the product of my ongoing keyboard layout hyperfixation, which started about two years ago from now. Vylet started out as a mod of [Wedlock](https://github.com/GGabi/wedlock) before evolving into its own thing. It takes inspiration from other alternative keyboard layouts like [APTv3](https://github.com/Apsu/APT), [Workman](https://workmanlayout.org/), and [Magic Sturdy](https://github.com/Ikcelaks/keyboard_layouts/blob/main/magic_sturdy/magic_sturdy.md). Vylet takes advantage of the following techniques/features:
- [Alt Fingering](#alt-fingering)
- [Sliding](#sliding)
- [Magic Key](#magic-key)

If you're not sure what any of those are, I've included some [definitions](#definitions) near the bottom of this readme to get you caught up.

## Goals / Vylet Features
By the time I started making my own mods/layouts in December 2023, I had already had a year of experience with [Colemak DH](https://colemakmods.github.io/mod-dh/), a month with [Canary](https://github.com/Apsu/Canary), and a bunch of weeks spread between a couple other layouts. Learning and typing daily with these different layouts was key in helping me find I wanted out of a layout. So when setting out to make one tailored to me, these were the characteristics I was aiming for:
- Balanced finger use
- High inrolls (with comparatively low outrolls)
- Low scissors (with little to no full scissors)
- Low LSBs
- Low index use, but only on the right hand (due to strain from mouse clicking)

All of these would be achieved with Vylet, and can be used to characterize what the layout is like. Here are some other notable characteristics of it:
- Low 2u SFS
- Balanced alternation (not low enough where you start getting too many onehands)

If you want to know more, feel free to check out the [analyzer data](analyzer_stats.md) I collected for Vylet from a few websites.

## Background
When doing my initial modding, I would tweak a letter's position every couple of days based on my comfort with it. I did this over the course of 2 months, and eventually realized I was making something very similar to APTv3. I had originally passed on learning this layout when I heard about it a year prior, but on second look it seemed like it had all the characteristics I was looking for. There was one exception though: the letter `Y`.

On APTv3, `Y` is placed on the top row of the right pinky. This would break my rules by introducing some nasty pinky-ring scissor interactions, as well as putting the pinky's usage above what I'd prefer. This is what got me thinking about where to place `Y`, and eventually deciding to optimize its placement based on alt fingering.

## Alt Fingering

The placement of `Y` in Vylet creates only 2 significant bigrams: `LY` and `NY`. Both of these bigrams can be alt fingered comfortably, which negates most of the SFBs this `Y` placement creates. We're just going to focus on `LY` since it's the more important SFB, and I tend to slide `NY` instead of alting it anyway.

Keep in mind that alt fingering doesn't just erase the total SFB percentage here (which is 0.377% in the Monkeyracer corpus). The `LY` alt finger starts with the right middle finger, meaning any word that uses a letter with this finger (`O` or `A`), followed by `LY` is still a SFB. This means words like `holy` or `really` contain SFBs in Vylet.

Taking this into account, the SFBs caused by `LY` in this layout isn't 0.377%, but instead is 0.091%.

## Sliding

`OA`, `UE`, and `PH` are all comfortable downwards slides for me. `NY` is also a slide, just a sideways one. It's worth mentioning that this technique doesn't work as well if you're on a standard mechanical keyboard with the taller, more spaced out keys. Low profile keyboards with light switches, and especially laptop keyboards are best suited for this.

## Magic Key

This leaves me with two significant SFBs in Vylet to address: `SC` and `WR`. I could slide `SC`, but upwards slides are much less comfortable than their downwards counterpart. `WR` is downwards, but is on the pinky which doesn't feel well-suited to do slides at least for my hands. This is why they would ultimately become rules for my magic key.

The magic key was a later addition to Vylet. It originally started as a way to fix the `SC` SFB and `CK` scissor, but has grown to be quite more useful than that.

### Magic Key Rules

Here is my full set of magic rules used in Vylet.

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

Most of these should be self-explanatory except the three `X` rules at the end. `X` can be annoying on the vowel side because in words, it's often between two other vowels (`exist`, `exactly`, `example`, etc.). This means any involvement of `X` in a word is likely going to be a redirect. These three rules make the redirects less of an issue since `X` is now in a closer, more comfortable spot.

My implementation of the magic key in my QMK config is done through [Sequence Transform](https://github.com/Ikcelaks/qmk_sequence_transform). It's what allows me to create magic rules with the extremely simple syntax you saw above. You can also do a bunch of other more complex things with it, I just don't take full advantage of that.

## Vylet Weaknesses

Personally I have very little issue with anything this layout has, but I do want to point out some factors that may be turnoffs for others.
- The hand balance leans right (46/54). If you're a right space user this could be too much.
- Depending on the analyzer used, redirects are either average or a bit above that.
- Vylet was not optimized with 1u SFS in mind, so the stat is only in the average range instead of being low like many modern layouts are.
- Some people can't get used to having a somewhat common letter like `W` on the top left pinky key.

## Definitions

- Alt Fingering: Pressing a key with a different finger than would be typed with traditional touch typing technique. An example of this on Qwerty would be using your middle finger and index finger to type `R` and `T` respectively for a word like `heart`. It can be used to make typing a SFB easier.
- Slide: Pressing a key and quickly moving to a neighboring key while not lifting your finger. An example of this on Qwerty would be sliding your middle finger from `E` down to `D` for a word like `walked`. It can be used to make typing a SFB easier.
- Magic Key: A key (often represended by `*` in layouts) which has an output based on the last keypress. The output, as well as what keys prompts said output, can be customized. An example would be this magic rule: `c★ ⇒ ck`. This rule indicates that if the last keypress before the magic key was `C`, the output will be `K`.

## Credits
The [Alt Keyboard Layouts (AKL) Discord](https://discord.com/invite/sxTV2G5Acg) for being extremely welcoming and teaching me more about keyboard layouts than I have any right to know.

[Cyanophage](https://cyanophage.github.io/index.html), [Pine](https://clemenpine.github.io/keysolve-web/), and [Oxey](https://oxey.dev/playground/index.html) for their web-based keyboard layout analyzers. Their ease of access has been invalable for me.

[Vylet Pony](https://www.youtube.com/@VyletPony) for inspiring the layout name, and for being the soundtrack to my keyboard layout brainrot.

[You](https://www.youtube.com/watch?v=heWXOUOcC3I) :D Thanks for reading!
