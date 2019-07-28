# srp_businesses
srp_businesses is a script that is based on Businesses from other GTA platforms such as SA:MP or RageMP. I've seen many server on those platforms having Businesses.
This business system was orginally developed for **StrefaRP.pl** If you do like our Businesses system give it a star! It'd be much appreciated <3

If you're feeleing generous<br>
<a href="https://paypal.me/pools/c/8g4D2PWQCG" rel="nofollow"><img src="https://camo.githubusercontent.com/d5d24e33e2f4b6fe53987419a21b203c03789a8f/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f6e6174652d50617950616c2d677265656e2e737667" alt="Donate" data-canonical-src="https://img.shields.io/badge/Donate-PayPal-green.svg" style="max-width:100%;"></a>

# Terms and conditions
I require only the following to anyone using this system:<br> **leave the script name as it is and do not sing it under ur own name.**
<br>For the rest, refer to the [license](https://github.com/Ezi2k/srp_businesses/blob/master/docs/LICENSE)

# How dose it work?
Our business system is user friendly.<br>
There are five administravie commands such as:
- /bizcreate (name) (marker id from 0 to 28) (price can't be lower then 25000$) (state 0 - For sale / 1 - sold / 2 - rented)
- /bizedit (business id) (name/owner/price/locker/interior/doors/state) (variabel)
- /bizdelete (business id)
- /bizinfo (debug command)
- /bizreload

## Features
- Business locker. (owner and co-workers can use open/close deposit and withdraw from the locker shuch items as: weapons/drugs ect.)
- Management zone (It's based on Society "boss" action menu. You can invite and kick players to or from ur businness)
- Locking doors (If you're a owner for a business and if you press **[L]** on your keyboard you will lock the doors. If doors are locked no one can entry or exit your business.)
- Entring the interior (If your business has an interior assigned then you can simply press **[E]** if the doors are unlocked then you will be teleported to the interior and from the same place you can press **[E]** once againg and you will be teleported from the interior.)
- Multi language support (Currently we're only supporting **Polish** and **English** but maybe in the future we will be supporting more languages.)

## Player commands
- /bizbuy (the player must stand in the business marker in order to work.)

## How to add new interiors?
It's pretty simple, you've to add new possitions and ID in "config.lua"<br> 
f.ex
```
{ id = 1, coords = { x = -781.97, y = 326.31, z = 223.26 } }
``` 
ID means the Interior id you will enter while editing the business with /bizedit (bussiness id) (interior) (and then id from config.lua)
<br>
coords are the coords player will be teleported to.

## How to change language?
It's really simple in "config.lua" you've line called 
```
lua Config.Locale = 'pl'
``` 
change it from pl to en and there you go!

<br>
**Command usage:

**
