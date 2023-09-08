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

 - <p id="Salamu"><b>Salamu, Dunia</b></p>
 
![image 1](CTFILP/General/1%20-%20Salamu%2C%20Dunia/1.png) 
<p>Soalan diberi <i>link website</i>.</p>
 
![image 2](CTFILP/General/1%20-%20Salamu%2C%20Dunia/2.png) 
<p>Bila di <i>click</i> ini adalah <i>content website</i> tersebut dan menyatakan bahawa hanya bahasa <b> Swahili </b> sahaja boleh mengekses kepada <i> content website </i> tersebut. Cuba akses dengan mengubah 
<i>cookies</i> website dengan bahasa <b>Swahili</b>. Menggunakan <i>Inspect Element - Tab Application - Cookies</i>.</p>
 
![image 3](CTFILP/General/1%20-%20Salamu%2C%20Dunia/3.png) 
<p> Disini kita dapat lihat data untuk cookies diberi nama <i> locale </i> dan <i>values</i> adalah <strong> 656E5F5553 </strong>. Apakah maksud <i>values</i> tersebut? Cuba <i> decrypt</i>. </p>
     
![image 4](CTFILP/General/1%20-%20Salamu%2C%20Dunia/4.png)      
<p> <i> Copy value</i> tersebut dan paste di <i><a href="https://www.cachesleuth.com/multidecoder/"> Multidecoder </a></i> tekan <i> Solve </i>.</p>
     
![image 5](CTFILP/General/1%20-%20Salamu%2C%20Dunia/5.png)      
<p> <i> Scroll </i> kebawah dan jumpa value yang tepat iaitu  <i> en_US </i>. Bermaksud ini adalah <i>value</i> bahasa menggunakan<i> encryption</i> <b> Hexadecimal. </b></p>

![image 6](CTFILP/General/1%20-%20Salamu%2C%20Dunia/6.png)  
<p> Pergi ke <i><a href="https://www.rapidtables.com/convert/number/hex-to-ascii.html"> Hexadecimal Decoder </a></i> dan <i>decode</i>, memang benar ini adalah  <i> values</i> bahasa <b>English</b>.</p>

![image 7](CTFILP/General/1%20-%20Salamu%2C%20Dunia/7.png)  
<p> Cari bahasa <b>Swahili</b> dalam bentuk <i> Code Language</i> dan <i> locale </i> : <b>sw_TZ </b>.</p>

![image 8](CTFILP/General/1%20-%20Salamu%2C%20Dunia/8.png) 
<p> Masukkan <i>value</i> <b>sw_TZ</b> dan <i>encrypt</i> kepada <b>Hexadecimal</b>. Copy <i>value</i> tersebut, <i>paste</i> di <i>value cookies</i> tekan <i>enter </i> dan <i>refresh</i>.</p>

![image 9](CTFILP/General/1%20-%20Salamu%2C%20Dunia/9.png)
<p>Dan ini adalah <b>flag</b>nya.</p>

- <p id="Gold"><b>Gold Digger</b></p>

![image 10](CTFILP/General/2%20-%20Gold%20Digger/1.png) 
<p>Soalan diberi <i>link website</i>.</p>

![image 11](CTFILP/General/2%20-%20Gold%20Digger/2.png) 
<p>Cuba dengan menggukan <i>command linux</i> iaitu <b>dig</b> dan <i>parameter <b>txt</b></i> untuk dapatkan info laman tersebut dan dapat <b>flag</b>.</p>

- <p id="Manage"><b>Flag Management System</b></p>

![image 12](CTFILP/General/3%20-%20Flag%20Management%20System/1.png) 
<p>Diberi adalah sebuah <i>folder</i>. <i>Download folder</i> tersebut.</p> 

![image 13](CTFILP/General/3%20-%20Flag%20Management%20System/2.png) 
<p><i>Extract folder</i> dan diberi adalah sebuah aplikasi berbentuk <i>EXE</i> dan <i> .Application</i> jadi ini adalah aplikasi <i>.NET</i>.</p> 

![image 14](CTFILP/General/3%20-%20Flag%20Management%20System/3.png) 
<p><i> Run </i> aplikasi tersebut. Ia memerlukan <i>username</i> dan <i>password</i>. </p> 

![image 15](CTFILP/General/3%20-%20Flag%20Management%20System/4.png) 
<p> <i> Disamble .NET</i> menggunakan <b>JetBrains dotPeek</b>. Pilih <i>process</i> aplikasi.</p>

![image 16](CTFILP/General/3%20-%20Flag%20Management%20System/5.png) 
<p> Dapat lihat <b> source code</b>.</p>

![image 17](CTFILP/General/3%20-%20Flag%20Management%20System/6.png) 
<p> Masukkan <i>username</i> dan <i>password</i>. Flag.</p>
