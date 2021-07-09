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
ℹ /DNS/TXT.TEXTPROTOCOL.ORG
ℹ /IP4/64.225.108.16/TCP/1968/NOISE
ℹ ℅ DIGITALOCEAN, FRANKFURT AM MAIN, HESSE 60313, GERMANY
ℹ ⧗ 18ms
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
ℹ 2021-07-09T11:05:03Z
ℹ 3DE5 488F 67AB F9CF
ℹ I02NM8
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
# '/bin/test' -t 1 2>/dev/null
# '/usr/bin/dig' +nocomments +nofail +ignore +short +retry=0 +notcp +time=1 +tries=1 $('/usr/local/bin/idn2' '_text._tcp.txt.textprotocol.org') TXT 2>/dev/null
# '/usr/bin/mktemp' -d -q 2>/dev/null
# '/usr/bin/mkfifo' 'tmp.nfReqHV7/01.result.fifo' 2>/dev/null
# '/usr/local/bin/timeout' 0.5 '/usr/local/bin/noisecat' -v -proto Noise_XX_25519_ChaChaPoly_BLAKE2b '64.225.108.16' 1968 1>'tmp.nfReqHV7/01.result.fifo' 2>/dev/null
# '/usr/bin/iconv' --from-code=UTF-8 --to-code=UTF-8 < 'tmp.nfReqHV7/03.status.txt' >/dev/null
# '/usr/bin/sed' 1d < 'tmp.nfReqHV7/02.response.raw' 1>'tmp.nfReqHV7/04.content.txt' 2>/dev/null
# '/usr/bin/file' --brief --mime-type --mime-encoding 'tmp.nfReqHV7/04.content.txt' 2>/dev/null
# '/bin/rm' -r 'tmp.nfReqHV7' 2>/dev/null
txt.textprotocol.org - - [2021-07-09T11:05:42Z] "text://txt.textprotocol.org/" 20 262
```

```bash
# textprint text://txt.textprotocol.org/elos.pdf
✂・・・・・・・・・・
ℹ /DNS/TXT.TEXTPROTOCOL.ORG
ℹ /IP4/64.225.108.16/TCP/1968/NOISE
ℹ ℅ DIGITALOCEAN, FRANKFURT AM MAIN, HESSE 60313, GERMANY
ℹ ⧗ 13ms
✂・・・・・・・・・・
✔ APPLICATION/PDF — 1,868 lines, 11,119 words, 80,088 characters, 157,962 bytes
ℹ UTF-8 ENG

                 William Strunk, Jr.
          The Elements of Style

…

```

```bash
# textprint text://txt.textprotocol.org/tatepon.png
✂・・・・・・・・・・
ℹ /DNS/TXT.TEXTPROTOCOL.ORG
ℹ /IP4/64.225.108.16/TCP/1968/NOISE
ℹ ℅ DIGITALOCEAN, FRANKFURT AM MAIN, HESSE 60313, GERMANY
ℹ ⧗ 18ms
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
ℹ 2021-07-09T11:07:34Z
ℹ D562 D083 E7B9 6AEB
ℹ I02NM8
```

```bash
# textprint text://txt.textprotocol.org/data.txt
✂・・・・・・・・・・
ℹ /DNS/TXT.TEXTPROTOCOL.ORG
ℹ /IP4/64.225.108.16/TCP/1968/NOISE
ℹ ℅ DIGITALOCEAN, FRANKFURT AM MAIN, HESSE 60313, GERMANY
ℹ ⧗ 18ms
✂・・・・・・・・・・
✔ TEXT/PLAIN — 6 lines, 9 words, 380 characters, 391 bytes
ℹ UTF-8

With embedded data: URI.

rel=icon
+--------------------------------+
|                                |
|                                |
|                                |
|                                |
|  ........  .      .  ........  |
| .::ckx::;..lc.   :o..;::xkc::. |
|    .xo     .oo,'ld.     ox.    |
|    .xo      .dNXx.      ox.    |
|    .xo      ;dood:      ox.    |
|    .xo    .ld'  .dl.    ox.    |
|     ,'    .;.    .;.    ';     |
|                                |
|                                |
|                                |
|                                |
|                                |
+--------------------------------+
image/png — 234 bytes — ascii

—
🆃🆇🆃

✂・・・・・・・・・・
ℹ 2021-07-09T11:08:09Z
ℹ F7B7 100E ABF4 0A2F
ℹ I02NM8
```

__DEPENDENCIES__

[ℹ︎](https://linux.die.net/man/1/base64 "base64(1) - man page")`base64`\
[ℹ︎](https://linux.die.net/man/1/clear "clear(1) - man page")`clear` _optional_\
[ℹ︎](https://linux.die.net/man/1/convert "convert(1) - man page")`convert` _optional_\
[ℹ︎](https://linux.die.net/man/1/date "date(1) - man page")`date` _optional_\
[ℹ︎](https://linux.die.net/man/1/dig "dig(1) - man page")`dig` _optional_\
[ℹ︎](https://linux.die.net/man/1/file "file(1) - man page")`file`\
[ℹ︎](https://linux.die.net/man/1/fold "fold(1) - man page")`fold`\
[ℹ︎](https://github.com/wooorm/franc "language detection")`franc` _optional_\
[ℹ︎](https://github.com/tomnomnom/gron "make json greppable")`gron` _optional_\
[ℹ︎](https://linux.die.net/man/1/iconv "iconv(1) - man page")`iconv`\
[ℹ︎](https://linux.die.net/man/1/idn2 "idn2(1) - man page")`idn2` _optional_\
[ℹ︎](https://csl.name/jp2a/ "converts images to ascii")`jp2a` _optional_\
[ℹ︎](https://linux.die.net/man/1/locale "locale(1) - man page")`locale`\
[ℹ︎](https://linux.die.net/man/1/lua "lua(1) - man page")__`lua`__\
[ℹ︎](https://linux.die.net/man/1/md5sum "md5sum(1) - man page")`md5sum` _optional_\
[ℹ︎](https://linux.die.net/man/1/mkfifo "mkfifo(1) - man page")`mkfifo`\
[ℹ︎](https://linux.die.net/man/1/mktemp "mktemp(1) - man page")`mktemp`\
[ℹ︎](https://github.com/maxmind/mmdbinspect "maxmind geoip")`mmdbinspect` _optional_\
[ℹ︎](https://linux.die.net/man/1/nc "nc(1) - man page")`nc`\
[ℹ︎](https://github.com/gedigi/noisecat "noisecat")`noisecat` _optional_\
[ℹ︎](https://linux.die.net/man/1/openssl "openssl(1) - man page")`openssl` _optional_\
[ℹ︎](https://linux.die.net/man/1/pdftotext "pdftotext(1) - man page")`pdftotext` _optional_\
[ℹ︎](https://linux.die.net/man/8/ping "ping(8) - man page")`ping` _optional_\
[ℹ︎](https://linux.die.net/man/1/rm "rm(1) - man page")`rm`\
[ℹ︎](https://linux.die.net/man/1/sed "sed(1) - man page")`sed`\
[ℹ︎](https://linux.die.net/man/1/tail "tail(1) - man page")`tail` _optional_\
[ℹ︎](https://linux.die.net/man/1/test "test(1) - man page")`test`\
[ℹ︎](https://linux.die.net/man/1/timeout "timeout(1) - man page")`timeout`\
[ℹ︎](https://linux.die.net/man/1/wc "wc(1) - man page")`wc`

