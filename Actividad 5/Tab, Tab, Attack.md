### Descripción: 
El uso de tabcomplete en la Terminal le agregará años a su vida, especialmente cuando se trata con estructuras de directorios y nombres de archivos largos y confusos: Addadshashanammu.zip
### Solución:
picoCTF{l3v3l_up!_t4k3_4_r35t!_a00cae70}
### Notas:
```shell
Morin-picoctf@webshell:~$ curl -O https://mercury.picoctf.net/static/a350754a299cb58988d6d47aed5be3ba/Addadshashanammu.zip
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  4521  100  4521    0     0  21335      0 --:--:-- --:--:-- --:--:-- 21426
Morin-picoctf@webshell:~$ unzip -l Addadshashanammu.zip
Archive:  Addadshashanammu.zip
  Length      Date    Time    Name
---------  ---------- -----   ----
        0  2021-03-16 01:16   Addadshashanammu/
        0  2021-03-16 01:16   Addadshashanammu/Almurbalarammi/
        0  2021-03-16 01:16   Addadshashanammu/Almurbalarammi/Ashalmimilkala/
        0  2021-03-16 01:16   Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/
        0  2021-03-16 01:16   Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/
        0  2021-03-16 01:16   Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/
        0  2021-03-16 01:16   Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/
     8320  2021-03-16 01:16   Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/fang-of-haynekhtnamet
---------                     -------
     8320                     8 files
Morin-picoctf@webshell:~$ unzip Addadshashanammu.zip
Archive:  Addadshashanammu.zip
   creating: Addadshashanammu/
   creating: Addadshashanammu/Almurbalarammi/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/
  inflating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/fang-of-haynekhtnamet  
Morin-picoctf@webshell:~$ ls -la
total 4256
drwxr-xr-x 5 Morin-picoctf Morin-picoctf   4096 Sep 13 17:17 .
drwxr-xr-x 3 root          root              27 Sep  1 16:32 ..
-rw------- 1 Morin-picoctf Morin-picoctf   3478 Sep 10 05:51 .bash_history
-rw-r--r-- 1 Morin-picoctf Morin-picoctf    220 Sep  1 16:32 .bash_logout
-rw-r--r-- 1 Morin-picoctf Morin-picoctf   3771 Sep  1 16:32 .bashrc
drwxrwxr-x 3 Morin-picoctf Morin-picoctf     27 Sep 10 06:21 .local
-rw-r--r-- 1 Morin-picoctf Morin-picoctf    807 Sep  1 16:32 .profile
drwx------ 2 Morin-picoctf Morin-picoctf     48 Sep 13 17:02 .ssh
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf    167 Sep 10 06:06 .wget-hsts
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf   7072 Sep 10 05:44 37
drwxr-xr-x 3 Morin-picoctf Morin-picoctf     36 Mar 16  2021 Addadshashanammu
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf   4521 Sep 13 17:17 Addadshashanammu.zip
-rw-r--r-- 1 root          root            4443 Sep 13 16:51 README.txt
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf      0 Sep 10 05:42 ]
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf 287372 Sep  1 17:39 bandera
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf  14551 Oct 26  2020 file
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf  61871 Sep  6 04:08 file.hex
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf     34 Mar 16  2021 flag
-rwxrwxr-x 1 Morin-picoctf Morin-picoctf    785 Sep 13 16:58 ltdis.sh
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf   8376 Sep 13 16:58 static
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf   1668 Sep 13 16:58 static.ltdis.strings.txt
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf   6497 Sep 13 16:58 static.ltdis.x86_64.txt
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf 776032 Oct 26  2020 strings
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf 776032 Oct 26  2020 strings.1
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf 776032 Oct 26  2020 strings.2
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf 776032 Oct 26  2020 strings.3
-rw-rw-r-- 1 Morin-picoctf Morin-picoctf 776032 Oct 26  2020 strings.4
-rwxrwxr-x 1 Morin-picoctf Morin-picoctf  10936 Mar 16  2021 warm
Morin-picoctf@webshell:~$ file *
37:                       HTML document, ASCII text, with very long lines (7072), with no line terminators
Addadshashanammu:         directory
Addadshashanammu.zip:     Zip archive data, at least v1.0 to extract, compression method=store
README.txt:               ASCII text, with escape sequences
]:                        empty
bandera:                  ASCII text
file:                     ASCII text, with very long lines (4200)
file.hex:                 ASCII text
flag:                     ASCII text
ltdis.sh:                 Bourne-Again shell script, ASCII text executable
static:                   ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=9f1762ab580608bef0d251f5fdfaad3d19ae0963, not stripped
static.ltdis.strings.txt: ASCII text
static.ltdis.x86_64.txt:  ASCII text
strings:                  ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=0cdedfba33422d235dba8c90e00fb77b235f1ff8, not stripped
strings.1:                ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=0cdedfba33422d235dba8c90e00fb77b235f1ff8, not stripped
strings.2:                ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=0cdedfba33422d235dba8c90e00fb77b235f1ff8, not stripped
strings.3:                ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=0cdedfba33422d235dba8c90e00fb77b235f1ff8, not stripped
strings.4:                ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=0cdedfba33422d235dba8c90e00fb77b235f1ff8, not stripped
warm:                     ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=b11c22752c901adc13ba1ce86eda9d5516f22763, with debug_info, not stripped
Morin-picoctf@webshell:~$ # Buscar directamente la bandera si es texto
Morin-picoctf@webshell:~$ grep -R -i 'picoCTF' *
37:<!DOCTYPE html><html lang="en-US"><head><title>Just a moment...</title><meta http-equiv="Content-Type" content="text/html; charset=UTF-8"><meta http-equiv="X-UA-Compatible" content="IE=Edge"><meta name="robots" content="noindex,nofollow"><meta name="viewport" content="width=device-width,initial-scale=1"><style>*{box-sizing:border-box;margin:0;padding:0}html{line-height:1.15;-webkit-text-size-adjust:100%;color:#313131;font-family:system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji"}body{display:flex;flex-direction:column;height:100vh;min-height:100vh}.main-content{margin:8rem auto;padding-left:1.5rem;max-width:60rem}@media (width <= 720px){.main-content{margin-top:4rem}}.h2{line-height:2.25rem;font-size:1.5rem;font-weight:500}@media (width <= 720px){.h2{line-height:1.5rem;font-size:1.25rem}}#challenge-error-text{background-image:url("data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIzMiIgaGVpZ2h0PSIzMiIgZmlsbD0ibm9uZSI+PHBhdGggZmlsbD0iI0IyMEYwMyIgZD0iTTE2IDNhMTMgMTMgMCAxIDAgMTMgMTNBMTMuMDE1IDEzLjAxNSAwIDAgMCAxNiAzbTAgMjRhMTEgMTEgMCAxIDEgMTEtMTEgMTEuMDEgMTEuMDEgMCAwIDEtMTEgMTEiLz48cGF0aCBmaWxsPSIjQjIwRjAzIiBkPSJNMTcuMDM4IDE4LjYxNUgxNC44N0wxNC41NjMgOS41aDIuNzgzem0tMS4wODQgMS40MjdxLjY2IDAgMS4wNTcuMzg4LjQwNy4zODkuNDA3Ljk5NCAwIC41OTYtLjQwNy45ODQtLjM5Ny4zOS0xLjA1Ny4zODktLjY1IDAtMS4wNTYtLjM4OS0uMzk4LS4zODktLjM5OC0uOTg0IDAtLjU5Ny4zOTgtLjk4NS40MDYtLjM5NyAxLjA1Ni0uMzk3Ii8+PC9zdmc+");background-repeat:no-repeat;background-size:contain;padding-left:34px}@media (prefers-color-scheme: dark){body{background-color:#222;color:#d9d9d9}}</style><meta http-equiv="refresh" content="360"></head><body><div class="main-wrapper" role="main"><div class="main-content"><noscript><div class="h2"><span id="challenge-error-text">Enable JavaScript and cookies to continue</span></div></noscript></div></div><script>(function(){window._cf_chl_opt = {cvId: '3',cZone: 'play.picoctf.org',cType: 'managed',cRay: '97cc9d63c8222237',cH: 'LBzN1j7e_09Og2sGA8WVgIx68kX790Zr5eTd8zagPBA-1757483080-1.2.1.1-OWVPfueDbQz7iW2SMU974wH8CNwp_N96SiSNFGiiT4kpThx3zAbI8LX6CqjnicHR',cUPMDTk:"\/practice\/challenge\/37?__cf_chl_tk=hsBcundRpgAnv0ajvg1B5C.R67Sfe19z8S7QzPMYSJ8-1757483080-1.0.1.1-V6oV4hqH1MQX4ADBy6sm4kB6LRjl_LhSSmrXxoSuggI",cFPWv: 'g',cITimeS: '1757483080',cTplC:0,cTplV:5,cTplB: 'cf',fa:"\/practice\/challenge\/37?__cf_chl_f_tk=hsBcundRpgAnv0ajvg1B5C.R67Sfe19z8S7QzPMYSJ8-1757483080-1.0.1.1-V6oV4hqH1MQX4ADBy6sm4kB6LRjl_LhSSmrXxoSuggI",md: '9pcdwRAFgIqy_5jujJ3z9OjJoQOC3wMxdkUk4.wq7WQ-1757483080-1.2.1.1-JV2boOsESQWTlURtJpORWR.jprJPcTegXADFvh3.AjQACe7RBG50eNlETyZcrhOp0wKrE4uJ4EhigxnzivT.03jPVHtatg6LITOfI_3hRFRmXL.IM0MNaIwba7Kzmut8d6NtAjs_pqX7OpISR21kl2ZNUtBPwr4E6YN7ZF56uKwNmpUA8AyPlHgsLy5bJpAfUo5aR0eA4YsZkiWskAsSPoVJmnU3D.VVbKm7D5YX.3i2klLrEwmWJ2jj7KHVKYa5zSVXIpPQDRtXba0Oxgy48tQiBJ3H67M0yuNgDk8SQzk..DoUpq0VoHp2ySX0XrPNGCgVPpmlS43JLjMN3x.5huoU5iiZDN_ieHxmpKfBE.B5Ww8ryvItOhunAl1LbiFbMaBQzLm8BCj0.LDANmnvgVsSE_17akuBSKoNUF3l4a_0OIopbBN4bkGtSn2_F2o_y8zXkowHofO5e3EBQKdPdQy6Hcn06Wv9Dp6bIGKFpuUORwIlezCER7eHjd059wWxDzMkib4tOcX7hgOUXX2ZSwzqumDqIOMeZAmTBRKz_E1GTh3ETMEDdgPhala5.hx9IgekP69eLE4kM0jIyVYfV7LUU2zTq9VfKfhbXEzwjwBP..2fCDapsOYuJd0HDLWZy21j6y8xevLt1pe0V4N6ftkUSls3aeEIg54a42JntcRWFROdg21NYgRP0SJkIKU.AGbjefUw3s__wviPGD9VGxuunHyAMa2VMLNjYs1tj20hqr5u4lk1qNsWr4e.xfmjqGNJvfcTpIkiiuxx6bMzZVRvdUo_bNqAKRARYe5hGbYbmRujLAJZA6CixNx7OJppVBmAJ55_0arCKxQDZOo1ZLPR68w_hRACzht2cBozeovY4XwmuY2xH7dniTDlSEVk_6W64A1wgKWq2kNkhl3yJHpRlWpViBUPE9njhyzUpwk',mdrd: 'RnnmbMC6eijwmAKkyRCbrhT4CbHingZcxM6N2J6CXAY-1757483080-1.2.1.1-j9PK5YGoVc45Vt1wCIHWK29AQ.h._7rZG9IJlMqn5SJ4xlPBTAHoKPuIv24jPNNR62YbmdWoIPEzuTbFAc_yUW86TjqUgvcvB7k8kY6iEXqBwlbgqfFXLXhPklD.fxEjfMyFwY_8fTni.rZ9hg9Q__PCL8TCJ2zf7tbhuc8RQ11IpRNVVtBLkSgUGLXzHkRcUT8GT9sSGoJxL5vCbF4o5sioBpVG4l8Sh9x45yYszqdCO.4ifbXALEiocrus9uVzBei362hYBuFozVwXgNMG_Muk9lup76otHAwMTKalP8ZJqX6Mtk0AFZkRTf5fjTYrh1UeAWqRlVA2BUwg_2Rnvs5d2qtSuGhVvHgpndx0q1vsGiwz6gGB.PoiV_hEkmZ.VvKHmebQ_.4qNlcJa5Nd58VjMJxohrQkV3gvyhWSQpnVpcMBS.UMB5SwYa.pbhzShw10hdQ4eThJ.QlHEOExpAtPZY_2I1D6AznQXIS69S00gEg7SknjY4G7keCMP.sjyU0TFTaCETmQTsMhshKGxGk3xgHuCjXCW2igkgB7bDXG2Coc3jpbDJ7yf6LjokbizfCLtPYyaRyqW9QazDkEsrtUAKpw7VJc_kdso.lX290sZfnIdlyVWMhjUcduntB_VAq9o3GvUWFtNrA1l7AOLJL3N7GY3eFakgYCZtUQ9zUeAuz9RDpCPAC9qBjwtpmtRkieJFDXr6r4NiUauFNhEAzM1jdWrubtVws4YGYFuTvOycQEZDHrMC6rsnXsUxWk5XYXTJX7rZ362X6jWudKEKfa8EE8xbxJlLKQ6kOA5FhFidesooVmpNiOId8XkN_fAoX0MtpVYz2Ic0z0P_UA7pJQK3H39Ejm8swalLOlnXm6xfzcNcaUvAe7L4SqFiDK8ScXqhqmImhCm6Lqlxr4gL3D3VDB_NUvf0_5Hfugr1g206gaD22_E9pXh56RV_5HySYTOYpFJOpZdXEqCb_Rr05ZP_LT0ZgpUhuOXXL4.fPuq8Sdmj6H9LLve92.nKPGUcr3eb5V7w7EBO3PYgtakc2M3d8SoFmoAuyINL1c9XFN53rthPqWj3XfekmC4PdLofN5oMvkT7V1P8dVrLZUE0HbvQZywb0qFvLhPA8ACnnqEMOjEp8_7RFZqrTVb.FPfiDwMXEqHojZC.XEleQvG2T1Ou_j5XDqDFz9DO4W88agSbZ4zt.6FNCnUFXWYHCzlwX7ccpyYLV8ASe6JLuiKwO5wJvB0gJJ_2fJdpQErdK1hntNEtZf0x2nkOl80IfXdfVMJf.fFzUDhbsSMhkp3qhJk0YPFk8pjuzdbhX9l0MJg9QcPIG7KWglfyb5zX7sjW3DThhpd7WkaGMVtmNB5AspgjQYHZa5.WidbwYThlPt0dc7sgAbmE7OuUJFacQwkzyxAStj2vf1qm438dC3uZq0UAKrPgQVxTWwWOw0idUtLa1UfmzU.Tq8icwRF7U55rG7QFKm6Yv74qiU6g0ZC5UhAobpkXx185S0FdxALKWbDmm9nmjpL2t4RJBgMunfPZMEyolyKZ9KYOotmkrshr4sRq0jjYr5w6rGLBioPSGPD9c.S3F6OWxQGtHmyJyJVtt64HrABoL4L8PyoZKROhepT.DydVGcZ8CoR8_ImntZXsHb9nvO9iGphee7MOToe1ku5QrwhrJBXJyLQLiRunf3xrmGHm6KHHC80gXf6M2f9mjZceLj3SHhyoJT8jzUwh8NDOxUsFMSFY.KEu6r84pwlyhGGizOagxA1tskSFhR0uEf48jIb632ycaFVllZCvKYb2s.ItKgADTXiJGIuYB.PR9d.2cSaxWqDnPzCkhJDMyY3L5xHcMdKTL4aLnlaHPmDlyLDwKBYhbMtVKNc1cSERsPNf2PaTmlVh51s_ZezmQqRoaQnJe21K0WAxvn2Wi5Bl3flYK7jmBdqgvR_nU7V_SEjX7u9OWpPk9ouQzYwCwJpw2CyyvcfdIN.89uAYETLTTBbKEnf3Kwba8wooEAcJVbLZxQdf39nkcRC0InjpF705H60SBKHK3ykQAl6UW0PuqyZxpE4hwS5IeZ._pTLTy6pqTB0u.K9zFgQSteChJ60TJ2STpsNMOtOaFe6cXVYHQlmgy7QJ7oCOd0NxXnZIRy2NE_ZM4VMgPLxheilljfc40l.vobFh0tEYt6GXPzvCGIskPQeZyY06HNUhmusMBv2FUiEhgEFb2Ze54okACy.smVaS607uC4PuvYWOJGThzO3uK1dAniILSimFO0byFDbrGZjd3E3wxprTkN6WPheBruvwW7imWlpVuiF5BKaC95tAKZ2W4k1hxihJgcGpPfkqiCalEp37BTC1MO3FhtlvZb5Km9IZAPs9dqNkCZGha7MGvCJp9vKWf2FuKm7M9UtUr2v6LTIS4yKV.LWf3is6GvNWSIXp3PuTaoBeJzTuJnHbJKhLj90Mf.6_DuTMxfltI0KgqcS90y2mo',};var a = document.createElement('script');a.src = '/cdn-cgi/challenge-platform/h/g/orchestrate/chl_page/v1?ray=97cc9d63c8222237';window._cf_chl_opt.cOgUHash = location.hash === '' && location.href.indexOf('#') !== -1 ? '#' : location.hash;window._cf_chl_opt.cOgUQuery = location.search === '' && location.href.slice(0, location.href.length - window._cf_chl_opt.cOgUHash.length).indexOf('?') !== -1 ? '?' : location.search;if (window.history && window.history.replaceState) {var ogU = location.pathname + window._cf_chl_opt.cOgUQuery + window._cf_chl_opt.cOgUHash;history.replaceState(null, null,"\/practice\/challenge\/37?__cf_chl_rt_tk=hsBcundRpgAnv0ajvg1B5C.R67Sfe19z8S7QzPMYSJ8-1757483080-1.0.1.1-V6oV4hqH1MQX4ADBy6sm4kB6LRjl_LhSSmrXxoSuggI"+ window._cf_chl_opt.cOgUHash);a.onload = function() {history.replaceState(null, null, ogU);}}document.getElementsByTagName('head')[0].appendChild(a);}());</script></body></html>
grep: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/fang-of-haynekhtnamet: binary file matches
README.txt:Welcome to the picoCTF webshell!
README.txt:picoCTF challenges.
README.txt:other@picoctf.org and we will consider adding it.
README.txt:  Extensive brute-forcing is not necessary to solve picoCTF challenges.
README.txt:- If you change your username through the picoCTF website, you will
bandera:picoCTF{digital_plumb3r_ea8bfec7}
file:picoCTF{grep_is_good_to_find_things_f77e0797}
flag:picoCTF{s4n1ty_v3r1f13d_4a2b35fd}
grep: static: binary file matches
static.ltdis.strings.txt:   1020 picoCTF{d15a5m_t34s3r_6f8c8200}
grep: strings: binary file matches
grep: strings.1: binary file matches
grep: strings.2: binary file matches
grep: strings.3: binary file matches
grep: strings.4: binary file matches
grep: warm: binary file matches
Morin-picoctf@webshell:~$ strings Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/fang-of-haynekhtnamet | grep picoCTF
*ZAP!* picoCTF{l3v3l_up!_t4k3_4_r35t!_a00cae70}
Morin-picoctf@webshell:~$ 
```
### Referencias:
Shell
