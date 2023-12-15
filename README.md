# My ergonomic keyboard setup 

I set out to find the best configuration for me. I chose [MoErgo"s glove80](https://www.moergo.com/) for the keyboard
and [zmk](https://zmk.dev/) to modify which keycode each physical key press sends to the system.
For the base layout I learnt that "qwerty" was designed to slow typists down so they wouldn"t jam their typewritters
and after some research I learnt about ["qgmlwb"](http://mkweb.bcgsc.ca/carpalx/?full_optimization) which seems to be the best layout.
I then extended "qgmlwb" to better suit the glove80"s peculiar shape and my specific needs;
I"m a software developer living in Montreal so I work in English and French and I wanted a solution that didn"t require me changing the keyboard"s language.
The final config is available [here](https://github.com/delriodev/zmk-config)
Th ^e rest of the article will go over how I extended zmk and my system"s k ymap to support french accents in an english keboard.

## The emitter 

zmk already define all except four of the character"s that I need, they are <accent-aigu>, <accent-grave>, <accent-circonflex>, <c-cedille>. 
Therefore, the first step was to fork [zmk"s character definitions]() and [extend them]().

[the guide](https://github.com/zmkfirmware/zmk/issues/177#:~:text=edited-,When%20I%20saw%20this,or%20%26kp%20SI_ZCAR.,-13%0A%20%20%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%0A%20%20%20%20%20%20%20%20%20%20%20%201%0A%20%20%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%0A%20%20%20%20%20%20%20%20%20%20%20%201)

[x] change arrows' order to be left, down, up, right
[x] move both layer keys one tile down 
[x] inverse '' and "" keys 
[ ] consider adding more keys at the bottom right key-board for special characters

space shift
bksp  ctrl
return alt
esc   rshift
del   gui

({[</
)}]>\
?!&|
=_-
"'`accent aigu ^ 
@# enne ccedille    
+*percent
