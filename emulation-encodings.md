# Wey Tec HK2000C Emulation Encodings

## Dealing 3000:
```
                     |   Cancel
        _Interupt____|___Orders_________
                     |
        _Contact_____|___Accept_________
        CMD | R/Up   |  R/Dn   | Inst
        Bid_|_Offer__|__I-Deal_|_Cancel_
           Zone      |       FMT
        ___YOURS_____|_______MINE_______
```

Scan codes generated:

|Emulation:   | PC    | SUN   |DEC EMU| D3000 | D2000 |RT EMU |WIN NT   | PC TERM |
|-------------|-------|-------|-------|-------|-------|-------|---------|---------|
|Key:         | EMU   | EMU   |!Alpha | EMU   |1/2 EMU|!EUREX |EMU GL-TR| EMU     |
|Interrupt    |       |       |       |       |       |       |         |         |
|Cancel Orders|       |       |       |       |       |       |         |         |
|Contact      |       |       |       |       |       |       |         |         |
|Accept       |       |       |       |       |       |       |         |         |
|CMD Bid      |       |       |       |       |       |       |         |         |
|R/Up Offer   |       |       |       |       |       |       |         |         |
|R/Dn I-Deal  |       |       |       |       |       |       |         |         |
|Inst Cancel  |       |       |       |       |       |       |         |         |
|Zone YOURS   |       |       |       |       |       |       |         |         |
|FMT MINE     |       |       |       |       |       |       |         |         |


CDR/EBS Quotron:
```    
                     |
        _Sell________|___Buy____________
                     |
        _Bid_________|___Offer__________
        Sell| North  |  Clear  | Buy
        Reg_|_ing____|__All____|_Reg____
           Off       |    
        ___All_______|___One____________

```

Scan codes generated:

```
|Emulation:   | PC    | SUN   |DEC EMU| D3000 | BL O  |  EBS  | D2000 |D2000/ |RT EMU |WIN NT   | PC TERM |
|Key:         | EMU   | EMU   |!Alpha | EMU   | EMU   |  EMU  | EMU   |1/2 EMU|!EUREX |         | EMU     |
|-------------|-------|-------|-------|-------|-------|-------|-------|-------|-------|---------|---------|
|Sell         |       |       |       |   *   |       |       |   *   |  *    |       |         |         |
|Buy          |       |       |       |       |       |       |       |       |       |         |         |
|Bid          |       |       |       |       |       |       |       |       |       |         |         |
|Offer        |       |       |       |       |       |       |       |       |       |         |         |
|Sell Reg     |       |       |       |       |       |       |       |       |       |         |         |
|North ing    |       |       |       |       |       |       |       |       |       |         |         |
|Clear All    |       |       |       |       |       |       |       |       |       |         |         |
|Buy Reg      |       |       |       |       |       |       |       |       |       |         |         |
|Off All      |       |       |       |       |       |       |       |       |       |         |         |
|One          |       |       |       |       |       |       |       |       |       |         |         |



|Emulation:   | PC    | SUN   |DEC EMU| D3000 | BL O  |  EBS  | D2000 |D2000/ |RT EMU |WIN NT    | PC TERM |
|Key:         | EMU   | EMU   |!Alpha | EMU   | EMU   |  EMU  | EMU   |1/2 EMU|!EUREX |          | EMU     |
|-------------|-------|-------|-------|-------|-------|-------|-------|-------|-------|----------|---------|
|F1           | F1    | F1    | F1   ±|   *   | F1   ±| Esc   |   *   |  *    |  F1  ±|    F1  ± | F1    ± |
|F2           | :     | :     | :    ±|       | :     | PgDn ±|       |       |   :   |     :    |         |
|F3           |       |       |      ±|       |       | F1   ±|       |       |       |          |         |
|F4           |       |       |      ±|       |       | F2   ±|       |       |       |          |         |
|F5           |       |       |      ±|       |       | F3   ±|       |       |       |          |         |
|F6           |       |       |      ±|       |       | F4   ±|       |       |       |          |         |
|F7           |       |       |      ±|       |       | 1    ^|       |       |       |          |         |
|F8           |       |       |      ±|       |       | 2    ^|       |       |       |          |         |
|F9           |       |       |      ±|       |       | ⌘#8  #|       |       |       |          |         |
|F10          |       |       |      ±|       |       | ⌘#5  #|       |       |       |          |         |
|F11          |  :    |  :    |  :   ±|       |  :    | ⌘#4  #|       |       |       |          |         |
|F12          | F12   | F12   | F12  ±|       | F12  ±| ⌘#3  #|       |       |  F12 ±|    F12 ± | F12   ± |
|F13          | ⇧F1   |       |       |       | F1 +  | ⌘     |       |       |       |    /↵   | ⇧F1  +  |
|F14          |  :    |       |       |       |x820102| PgUp ±|       |       |       |   ⌃⌘.   |0x820102 |
|F15          |       |       | F13  ±|       |   :   | F7   ±|       |       |       |          |         |
|F16          |       |       | F15  ±|       |       | F8   ±|       |       |       |    %    !|         |
|F17          |       |       |0x6e   |       |       | F9   ±|       |       |       |    7    !|         |
|F18          |       |       |       |       |       | F10  ±|       |       |       |    =    !|         |
|F19          |       |       |       |       |       | 3    ^|       |       |       |    (    !|         |
|F20          |       | =    §|       |       |       | ⌘#2  .|       |       |       |    )    !|         |
|F21          |       |       |0x47  ±|       |       | ⌘#6  #|       |       |       |    _    !|         |
|F22          |       |       |0x4b  §|       |   :   | ⌘#8  ^|       |       |       |    @    !|         |
|F23          |   :   |       |0x43  §|       |x820102| ⌘#9  #|       |       |       |     [    |0x820102 |
|F24          | ⇧F12 | F13  ±|0x4e  §|       | + F12 | ⌘#0  .|       |       |       |     =↵  | + ⇧F12  |
|--------     | ---   | ---   | ---   |       |       |       |       |       |       |          |         |
|Print        | F13   | F13   |       |       | F13  ±| F13  ±|       |       |       |          |         |
|Scroll Lock  | F14   | F14   |0x6b  ±|       | F14  ±| F14  ±|       |       |       |          |         |
|Pause        | F15   | F15   |       |       | F15  ±| F15  ±|       |       |       |          |         |
|Ins          | Help  | Help  |Help  †|       | Help §| Help †|       |       |       |          |         |

    ! = + modifier 0x020102
    . = + modifier 0x100108
    § = + modifier 0x200100
    # = + modifier 0x300108
    ^ = + modifier 0x040101
    ± = + modifier 0x800100
    † = + modifier 0xc00100


    PC EMU --     F1-F12 keys labeled on LCD
    D3000 EMU --  No F keys work. No other keys on the kbd work. No plug-in module keys work.
    BL O EMU --   F1=Help, F2=Govt, = Corp, =Mtge, =MMkt, =Muni, =PFD, =Eqty, =CMDT, =Indx, F11=CRNC, F12=Clnt
    D2000 EMU --  No F keys work. No other keys on the kbd work. No plug-in module keys work.
```
