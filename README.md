![image info](CTFILP/368214536_1269997957221253_7629467549862697930_n.jpg)

<h1> WRITE UP CTF ILP </h1>
<p>Pertandingan <b>"CAPTURE THE FLAG" Unleash The Cyber Warrior</b>.</p>
<p>Diadakan di Institut Latihan Perindustrian Kuala Langat sempena program MINGGU KESELAMATAN SIBER ILP KUALA LANGAT.</p>

<HR>

+ <b><a href="#GENERAL"><strong>GENERAL</strong></a></b>
    - <a href="#Salamu">Salamu, Dunia</a>
    - <a href="#Gold">Gold Digger</a>
    - <a href="#Manage">Flag Management System</a>
    - <a href="#Admin">Be The Admin</a>
    - <a href="#Mystification">Mystification</a>
    - <a href="#Slow">Slow Internet</a>

+ <b><a href="#STOLEN">STOLEN</a></b>
    - <a href="#Whobad">Who is the bad guy?</a>

 + <b><a href="#HACKED">HACKED</a></b>
    - <a href="#hack1">Hacked 1</a>
    - <a href="#hack2">Hacked 2</a>
    - <a href="#hack3">Hacked 3</a>
    - <a href="#hack4">Hacked 4</a>
    - <a href="#hack5">Hacked 5</a>
    - <a href="#hack6">Hacked 6</a>
    - <a href="#hack7">Hacked 7</a>

 + <b><a href="#TRIVIA">TRIVIA</a></b>
    - <a href="#puisi">Puisi</a>
    - <a href="#hiding">Hiding</a>
    - <a href="#supper">Supper</a>
    
 + <b><a href="#GENERALS">.GENERAL</a></b>
    - <a href="#pocket">Pocket Dial</a>

# <h2 id="GENERAL"><strong>GENERAL</strong></h2>

 - <h3 id="Salamu"><b>Salamu, Dunia</b></h3>
 
![image 1](CTFILP/General/1%20-%20Salamu%2C%20Dunia/1.png) 
<p>Soalan diberi <i>link website</i>.</p>
 
![image 2](CTFILP/General/1%20-%20Salamu%2C%20Dunia/2.png) 
<p>Bila di <i>click</i> ini adalah <i>content website</i> tersebut dan menyatakan bahawa hanya bahasa <b> Swahili </b> sahaja boleh mengakses kepada <i> content website </i> tersebut. Cuba akses dengan mengubah 
<i>cookies</i> website dengan bahasa <b>Swahili</b>. Menggunakan <i>Inspect Element - Tab Application - Cookies</i>.</p>
 
![image 3](CTFILP/General/1%20-%20Salamu%2C%20Dunia/3.png) 
<p> Disini kita dapat lihat data untuk cookies diberi nama <i> locale </i> dan <i>values</i> adalah <strong> 656E5F5553</strong>. Apakah maksud <i>values</i> tersebut? Cuba <i> decrypt</i>. </p>
     
![image 4](CTFILP/General/1%20-%20Salamu%2C%20Dunia/4.png)      
<p> <i> Copy value</i> tersebut dan <i>paste</i> di <i><a href="https://www.cachesleuth.com/multidecoder/"> Multidecoder </a></i> tekan <i> Solve</i>.</p>
     
![image 5](CTFILP/General/1%20-%20Salamu%2C%20Dunia/5.png)      
<p> <i> Scroll </i> kebawah dan jumpa value yang tepat iaitu  <i> en_US</i>. Bermaksud ini adalah <i>value</i> bahasa menggunakan<i> encryption</i> <b> Hexadecimal. </b></p>

![image 6](CTFILP/General/1%20-%20Salamu%2C%20Dunia/6.png)  
<p> Pergi ke <i><a href="https://www.rapidtables.com/convert/number/hex-to-ascii.html"> Hexadecimal Decoder </a></i> dan <i>decode</i>, memang benar ini adalah  <i> values</i> bahasa <b>English</b>.</p>

![image 7](CTFILP/General/1%20-%20Salamu%2C%20Dunia/7.png)  
<p> Cari bahasa <b>Swahili</b> dalam bentuk <i> Code Language</i> dan <i> locale </i> : <b>sw_TZ </b>.</p>

![image 8](CTFILP/General/1%20-%20Salamu%2C%20Dunia/8.png) 
<p> Masukkan <i>value</i> <b>sw_TZ</b> dan <i>encrypt</i> kepada <b>Hexadecimal</b>. Copy <i>value</i> tersebut, <i>paste</i> di <i>value cookies</i> tekan <i>enter </i> dan <i>refresh</i>.</p>

![image 9](CTFILP/General/1%20-%20Salamu%2C%20Dunia/9.png)
<p>Dan ini adalah <b>flag</b>nya.</p>

- <h3 id="Gold"><b>Gold Digger</b></h3>

![image 10](CTFILP/General/2%20-%20Gold%20Digger/1.png) 
<p>Soalan diberi <i>link website</i>.</p>

![image 11](CTFILP/General/2%20-%20Gold%20Digger/2.png) 
<p>Menggunakan <i>linux</i> iaitu <b>dig</b> dan <i>parameter <b>txt</b></i> untuk dapatkan info laman tersebut dan dapat <b>flag</b>.</p>

- <p id="Manage"><h3>Flag Management System</b></h3>

![image 12](CTFILP/General/3%20-%20Flag%20Management%20System/1.png) 
<p>Diberi adalah sebuah <i>folder</i>. <i>Download folder</i> tersebut.</p> 

![image 13](CTFILP/General/3%20-%20Flag%20Management%20System/2.png) 
<p><i>Extract folder</i> dan diberi adalah sebuah aplikasi berbentuk <i>EXE</i> dan <i> .Application</i> jadi ini adalah aplikasi <i>.NET</i>.</p> 

![image 14](CTFILP/General/3%20-%20Flag%20Management%20System/3.png) 
<p><i> Run </i> aplikasi tersebut. Ia memerlukan <i>username</i> dan <i>password</i>. </p> 

![image 15](CTFILP/General/3%20-%20Flag%20Management%20System/4.png) 
<p> <i> Disamble .NET</i> menggunakan <b>JetBrains dotPeek</b>. Pilih <i>process</i> aplikasi.</p>

![image 16](CTFILP/General/3%20-%20Flag%20Management%20System/5.png) 
<p> Dapat lihat <b> source code</b>.  Masukkan <i>username</i> dan <i>password</i>.</p>

![image 17](CTFILP/General/3%20-%20Flag%20Management%20System/6.png) 
<p> Flag.</p>

- <h3 id="Admin"><b>Be The Admin</b></h3>

![image 18](CTFILP/General/4%20-%20Be%20the%20admin/1.png) 
<p>Soalan diberi <i>link website</i> serta <i>hint</i> mengatakan hanya <i>admin</i> sahaja boleh <i>akses</i>.</p>

![image 19](CTFILP/General/4%20-%20Be%20the%20admin/2.png) 
<p><b>SQL Injection</b> dengan menggunakan keyword <code><b>Admin' #</b></code> sebagai <i>username</i> dan <i>password</i> boleh diisi apa sahaja.</p>

![image 20](CTFILP/General/4%20-%20Be%20the%20admin/3.png) 
<p>Flag.</p>

- <h3 id="Mystification"><b>Mystification</b></h3>

![image 21](CTFILP/General/5%20-%20Mystification/1.png) 
<p>Soalan diberi <i>link website</i>.</p>

![image 22](CTFILP/General/5%20-%20Mystification/2.png) 
<p><i>View Source Code website</i> dan dapat lihat jika <i>username</i> dan <i>password</i> betul akan memanggil <b>flag<b> <i>function</i>.</p>

![image 23](CTFILP/General/5%20-%20Mystification/3.png) 
<p>Cari <b>flag<b> <i>function</i>.</p>

![image 24](CTFILP/General/5%20-%20Mystification/4.png) 
<p><b>Run alert<b> <i>function</i> di <i>Javascript Compiler</i> dan dapat <b>flag</b>.</p>

- <h3 id="Slow"><b>Slow Internet</b></h3>

![image 25](CTFILP/General/6%20-%20Slow%20Internet/1.png)
<p>Diberi adalah sebuah <i>folder PCAPNG</i>. <i>Download folder pcapng</i> tersebut.</p> 

![image 26](CTFILP/General/6%20-%20Slow%20Internet/2.png)
<p>Buka menggunakan <i>WIRESHARK</i> dan semak semua <i>info</i> pada <i>protocol DNS</i> terdapat <i>info</i> tersebut.</p> 

![image 27](CTFILP/General/6%20-%20Slow%20Internet/3.png)
<p><i>Copy</i> semua  <i>info</i> tersebut.</p> 

![image 28](CTFILP/General/6%20-%20Slow%20Internet/4.png)
<p><i>Copy encryption</i> yang pertama <i>info</i> tersebut dan <i>paste</i> di <i><a href="https://www.cachesleuth.com/multidecoder/"> Multidecoder </a>.</p> 

![image 29](CTFILP/General/6%20-%20Slow%20Internet/5.png)
<p><i>Encryption</i> adalah <b>base32</b> : <b> NasiAyamKakWok</b>.</p> 

![image 30](CTFILP/General/6%20-%20Slow%20Internet/6.png)
<p>Gabung semua <i>Encryption</i> dari 1 hingga 8, <i>paste</i> di <i><a href="https://www.dcode.fr/cipher-identifier"> Cipher Identifier </a></i>.</p> 

![image 31](CTFILP/General/6%20-%20Slow%20Internet/7.png)
<p>Result adalah sebuah <i>folder</i>. <i>Download folder</i>.</p> 

![image 32](CTFILP/General/6%20-%20Slow%20Internet/8.png)
<p>Terdapat <i>flag file</i>, masukkan <i>password</i> yang di<i>encrpt</i> awal : <b> NasiAyamKakWok</b>.</p>

![image 33](CTFILP/General/6%20-%20Slow%20Internet/9.png)
<p><b>Flag</b>.</p>

<p>Maklumat:</p>
```A 01-JZQXG2KBPFQW2S3BNNLW62YK - NasiAyamKakWok

01-KBFQGBAKAAEQAAAAGKYSEV35C4DB4NIAAAACSAAAAAEAAHAAMZ \zqu"vqpzppt"ppppvz*$t'bdrcsqc}xppppr$ppppptppwpp|+
 02-WGCZZOOR4HIVKUBEAAHX7K6NSNN2XTMR2XQCYAAECOQAYAAACO 
03-QAYAAA546JIBXPIZM5VRXMLWEWB56MVZJUCOJ2PQN5IQHPIEEM 
04-YYKMV556FCSTYKXVWTAGRH6TAXFHGSW2NNLQQ7M4SQJMDQQ7IX 
 05-AYPDKAAAAAUQAAAAKBFQCAQ6AMFAACIAAAADFMJCK56ROBQ6GU 
 06-AAAABJAAAAACAADAAAAAAAAAAQAAAAUSAQAAAAABTGYYLHFZ2H 
 07-Q5CVKQCQAA675LZWI5LYBMAACBHIAMAAABHIAMAAAUCLAUDAAA 
 08-AAAAAQAAIAJYAAAAEHAAAAAAAA ppppp"ppxpy*pppptwpppppppp


A 01-JZQXG2KBPFQW2S3BNNLW62YK - NasiAyamKakWok

KBFQGBAKAAEQAAAAGKYSEV35C4DB4NIAAAACSAAAAAEAAHAAMZWGCZZOOR4HIVKUBEAAHX7K6NSNN2XTMR2XQCYAAECOQAYAAACOQAYAAA546JIBXPIZM5VRXMLWEWB56MVZJUCOJ2PQN5IQHPIEEMYYKMV556FCSTYKXVWTAGRH6TAXFHGSW2NNLQQ7M4SQJMDQQ7IXAYPDKAAAAAUQAAAAKBFQCAQ6AMFAACIAAAADFMJCK56ROBQ6GUAAAABJAAAAACAADAAAAAAAAAAQAAAAUSAQAAAAABTGYYLHFZ2HQ5CVKQCQAA675LZWI5LYBMAACBHIAMAAABHIAMAAAUCLAUDAAAAAAAAQAAIAJYAAAAEHAAAAAAAA - LINK```
