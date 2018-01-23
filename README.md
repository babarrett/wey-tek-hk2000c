# WEY-TEK-HK2000C

Starting with a todo list for now.

## Email to Photoelectric:

* Bought my own: WEY HK2000C. To arrive this week.
* Connector Box Va
* EBS and Dealing add-on modules (10 keys each arranged with 2,2,4, and 2 keys
per row.) The keyboard is connected to each plug-in module with a 10 wire connector. 
```
        Dealing 3000:
                     |   Cancel
        _Interupt____|___Orders_________
                     |
        _Contact_____|___Accept_________
        CMD | R/Up   |  R/Dn   | Inst
        Bid_|_Offer__|__I-Deal_|_Cancel_
           Zone      |       FMT
        ___YOURS_____|_______MINE_______
    
        CDR/EBS Quotron:
                     |
        _Sell________|___Buy____________
                     |
        _Bid_________|___Offer__________
        Sell| North  |  Clear  | Buy
        Reg_|_ing____|__All____|_Reg____
           Off       |    
        ___All_______|___One____________

```

* The keyboards are preconfigured to work with six PC workstations on ports
USB1–USB6.
* Ebay URL: https://www.ebay.com/itm/HK2000C-KEYBOARD-kit-refurbished/172995887269
* I tried again signing up for an account to access tech documents at
weytec.com. This time I heard back. I got the firmware download application from
WEY Tec, happy to send you a copy. (Haven't tried it out yet. Don't know which
Windows OS it works with.)
* I still haven't seen a doc on the interface to the add-on modules. Now I'm
(mildly) considering leaving the 16 button add-on in place (for looks and to
avoid a big hole), but disconnecting it. Then simulate it using an outboard
macro pad for the left side of the keyboard. Quite a ways off.
* I'll try emulation modes other than "PC" to see if I can get more scan codes.
* Cable from keyboard to controller box, listed as a "half pitched centronics
cable" on page 18/49 of the manual. http://www.pchcables.com/hhaceprca.html
* Here's the English manual of the MK06: 
https://drive.google.com/open?id=0B3l12...3d4dU1MSjQ


## Things to find out / do, learning about this keyboard:

* Connect box, USB to hub, power cord, power strip
* USB A to USB A for host 
* Remove sw. Karabiner, Hammerspoon, sticky keys. 
* Mac = USA Kbd 
* PC emu on kbd
* Record (103?) scan codes using copy of G80-9000 layout
* In PC emulation mode, are keys/scan-codes sent for the "non-standard/PC" keys?
For example the color add-in modules, F13-F24, Attach, ... **No**, not when in
PC emulation mode. **TBD** What about other emulation modes?
* Test lock window behavior: Caps, Num, Scroll
* Re-test for extended scan-codes for other emulations. (Sun, Trading devices, etc.)
* (The Wey MK06 has a test mode that will display (on the keyboard) the scan code
resulting from pressing each key on the plug-in modules.)
* Switch to USB 2-5, try again
* Switch to host (USB 6), try again
* Change to EMU #1, retry work station scan codes. 
* See if there is a scan  code test mode.
* Load & save set-up to/from controller. Should be built in. Should be easy.
    * Change back, save settings in box
* Repeat with EMU #2, iterate
* Install USB mouse in "Host" (S6) port and see if it's signals are passed onto the PCs.
* Plug a shared (PS/2) mouse directly into the Kbd. Looks like that will get
forwarded to the active workstation, correct? **TBD** Interfaces include:
    * Serial (docs say: "RS232 compatible interface and MS-Mouse protocol")
    * PS/2
    * USB (yes, for HK2000C)
* The keyboard is connected to each plug-in module with a 10 wire connector.
This supports up to 16 keys. There are 4 diodes on the board (or, less likely in
keyboard) that determine the plug-in module type. 16 in total.
* Swap kbds, repeat
* Swap connect boxes


* Determine the use of these  10pins, here are a couple theoretical possibilities:
```
        Sample #s   Use
        ---------   ------------------------------------------------
        1-5:        5 bit to 32 decoder
                        4:  for the ID sensors, yields x00 to x0F IDs
                        16: for the (up to) 16 keys
        6:          Sense line for all of the above.
        7:          Power
        8:          Ground
        9-10:       Spare?
    
        1-4:        for the ID sensors
        5-8:        4 bit to 16 decoder
        9:          Sense line
        10:         ?
```

## To buy:

* (Have, somewhere): 2 standard PC power plugs
* (Have, somewhere): 1 more powerstrip to power off switch for the 2nd kbd.
* (Have, somewhere): At least one USB-A to USB-B
* √ Amazon: 6 short USB cables for simultaneous access to the 6 WS ports on a USB
hub. Possible max of 12 in total later, TBD.
* Sent -- Email to Andreutech - Can I get a blank too? (No reply)
* Hsau's USB-to-USB adapter
* (Future) Carrying case for keyboard

## To Try



## To research / learn:

* What's the Host port on the connector box do?
* What are the specs for the add-on modules?
    * Hardware (connector, size, etc.)
    * Software (what choices for modules do I have?)
* How do I load new/different software into the keyboard for a different module?
* Can Hsau's USB-to-USB be placed between a hub and PC to merge 6 keyboards,
through the same transform, into one?


## From Andreutech (NY)

1.	The keyboards are HK2000C with PS/2, USB and serial ports. 
2.	The controllers are all Connector Box Va with the latest firmware
3.	EBS and Dealing add-on modules in each
4.	The standard PC power cords can be used on the power supply
5. The keyboards are preconfigured to work with six PC workstations on ports
USB1–USB6. All the keyboards and connector boxes have the latest firmware
installed.

## Future:

* Make a 10 to 16-key "side-car" for the left side if the case (G80-9009 has 14 on
left that the Wey does not.) KLE: http://www.keyboard-layout-editor.com/#/gists/ed5696678d6d7faf714954512a94756d

## Owners:

### Deskthority Wey MK06:
```
  https://deskthority.net/photos-f62/wey-technology-mk06-t15102.html
  Wodan
  Chyros
  ting
  Orpheo
```

### Geekhack:

```
  Samuelll101 (MK06)
  dorkvader (HK2000C since 2014)
  xavierblak (HK2000C)
  Photoelectric (HK2000C)
  
```

3M Cable Connectors: 
  http://www.newark.com/3m/10136-3000pe/mini-d-ribbon-conn-plug-36pos/dp/69K7226

Power supply connector:
  https://www.digikey.com/product-detail/en/PDP-30/CP-7330-ND/2119403

Drivers:
  Controller box: are Torx T6. I have a spare I can send you if you need. They
aren't even pentalobe, torxplus or securitorx(harder to get).

Keyboard itself needs a T6 to open up and a T8 to get the controller off.
