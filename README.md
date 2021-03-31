# PUBLIC
[NETCAT](https://en.wikipedia.org/wiki/Netcat "NETCAT") [TEXT://PROTOCOL](https://textprotocol.org "TEXT://PROTOCOL") CLIENT

```bash
--
-- public
-- netcat text://protocol client
--
-- # textprint() { public "$1" 2>/dev/null; }
-- # textsource() { public "$1" 2>/dev/null | tee; }
-- # textlog() { public "$1" 1>/dev/null ; }
--
```

```bash
# textprint text://txt.textprotocol.org/
✂・・・・・・・・・・
ℹ /DNS/TXT.TEXTPROTOCOL.ORG/TCP/1961
ℹ /IP/165.22.70.231/TCP/1961
ℹ ℅ DIGITALOCEAN, FRANKFURT AM MAIN, HESSE 60313, GERMANY
ℹ ⧗ 15ms
✂・・・・・・・・・・
ℹ ✖ HOSTED ✖ SIGNED ✖ ENCRYPTED
✂・・・・・・・・・・
✔ TEXT/PLAIN — 9 lines, 20 words, 251 characters, 262 bytes
ℹ UTF-8

TEXT://PROTOCOL

geo:37.429167,-122.138056 PALO ALTO, CA 94301, USA
tag:txt.textprotocol.org,2021-03-07:~lablyd-dolben rel=me
text://txt.textprotocol.org/icon.png rel=icon
text://txt.textprotocol.org/license.txt rel=license CC0-1.0

—
🆃🆇🆃

✂・・・・・・・・・・
ℹ 2021-03-29T15:27:58Z
ℹ BFD1 A8E8 9740 F159
ℹ 19T0ANB
```

```bash
# textprint text://txt.textprotocol.org/tatepon.png
✂・・・・・・・・・・
ℹ /DNS/TXT.TEXTPROTOCOL.ORG/TCP/1961
ℹ /IP/165.22.70.231/TCP/1961
ℹ ℅ DIGITALOCEAN, FRANKFURT AM MAIN, HESSE 60313, GERMANY
ℹ ⧗ 15ms
✂・・・・・・・・・・
ℹ ✖ HOSTED ✖ SIGNED ✖ ENCRYPTED
✂・・・・・・・・・・
✔ IMAGE/PNG — 11,967 bytes
ℹ ASCII

MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
MMMMMMMMMMMMMMMMMo'lNMMW0WMMMMMMMMMMMMMMMMMMMM
MMMMMMMMMMMMMMMMM.  .NX. ,MMMMMMMMMMMMMMMMMMMM
MMMMMMMMMMMMN'.lX:   :l   XMMMMMMMMMMOx0WMMMMM
MMMMMMMMMMMMW,   d.   :   XMMMMMMMMMMX.  ;KMMM
MMMMMMNXKNMMMN:   c   '  .WMMMMMMMMMMM,    :NM
MMNd,',;;,',oNMx   ,  .. .lcNMMMM0:lkc  .   :M
Md.;KMMMMMMK:.kNd  .        :0WMM0    lWMMXxoM
k dMMMMNWMMMMc c        ..'.. .;kWK:   0MMMMMM
:.WMMMO..OMMMK .     ,kXk:,',;:; .0MNkl;kOKMMM
l NMN: ,c .lK0      kM0.       .k. xMMMx   :MM
K ;o..kWMWk:.      dMM:         l0  OMMX, ,,0X
Mx  kWMMMMMM0      0MMx         ON  cMMK.xMx,O
MMO.:WMMMMMX.      cMMM0:.   .cXMx  ;k:,OMMMMM
MMMX'.0MMMW, ,      :NMMMMWNWMMWo   cxXMMMMMMM
MMMMWc oMMl dx:       ;d0XXX0x;   .OMMMMMMMMMM
MMMMMMk.:x lMMMO.                ;XMMMMMMMMMMM
MMMMMMMK. .NMMMMWk:.          .lKMMMMMMMMMMMMM
MMMMMMMMN,0MMMMMMMMMXd :lc lONMMMMMMMMMMMMMMMM
MMMMMMMMMMMMMMMMMMMMMO.WMW.kMMMMMMMMMMMMMMMMMM
MMMMMMMMMMMMMMMMMMMMMk.MMW.xMMMMMMMMMMMMMMMMMM
MMMMMMMMMMMMMMMMMM0cc:cMMW::ccxMMMMMMMMMMMMMMM
MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM

✂・・・・・・・・・・
ℹ 2021-03-31T11:11:11Z
ℹ D58E A7E1 841D A368
ℹ 19T0ANB
```

```bash
# textsource text://txt.textprotocol.org/
20 text/plain; charset=utf-8; content-length=262
TEXT://PROTOCOL

=> geo:37.429167,-122.138056 PALO ALTO, CA 94301, USA
=> tag:txt.textprotocol.org,2021-03-07:~lablyd-dolben rel=me
=> text://txt.textprotocol.org/icon.png rel=icon
=> text://txt.textprotocol.org/license.txt rel=license CC0-1.0

—
🆃🆇🆃
```

```bash
# textlog text://txt.textprotocol.org/
# '/usr/bin/locale' charmap 2>/dev/null
# '/bin/test' -t 1 2>/dev/null
# '/usr/bin/dig' +nocomments +nofail +ignore +short +retry=0 +notcp +time=1 +tries=1 $('/usr/local/bin/idn2' 'txt.textprotocol.org') A 2>/dev/null
# '/usr/local/bin/timeout' 5 '/usr/bin/nc' -C -G 5 -w 5 '165.22.70.231' 1961 <<< 'text://txt.textprotocol.org/' 2>/dev/null
# '/usr/bin/iconv' --from-code=UTF-8 --to-code=UTF-8 < '02.status.txt' >/dev/null
# '/usr/bin/sed' 1d < '01.response.raw' 1>'03.content.txt' 2>/dev/null
# '/usr/bin/file' --brief --mime-type --mime-encoding '03.content.txt' 2>/dev/null
```


