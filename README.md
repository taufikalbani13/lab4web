# lab4web

#  Nama : Taufik Eka Albani
#  Nim  : 312210347
#  Kelas: TI.22.A3

## 1). MEMBUAT DOKUMEN HTML DENGAN NAMA lab4_box.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
</head>
<body>
    <header>
        <h1>Box Element</h1>
    </header>
</body>
</html>
```

## 2). MEMBUAT BOX ELEMENT

## CONTOH CODE DAN TAMPILAN BROWSER NYA!


**PENJELASAN** 

Disitu sudah terdapat section dengan tag div yang kemudian diberi Deklarsi **CSS INTERNAL** dan ***property Float***

***code html***
```html
<section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
    </section>
```

***code css***
```css
    <style>
        div{
            float: left;
            padding: 10px;
        }
        .div1{
            background: red;
        }
        .div2{
            background: yellow;
        }
        .div3{
            background: green;
        }
    </style>

```
## 3). MENGATUR CLEARFIX ELEMENT

## CONTOH CODE DAN TAMPILAN BROWSER NYA!


**PENJELASAN**

Disitu ditambahkan tag **div4** kembali dan kemudian dibuat dan dideklarasikan di ***css internal*** dengan ***property clear: right*** dan juga ***float:none*** saya melakukan eksperimen dengan menjadikan nya **right** dan gambar diatas adalah contoh nya.

**code html**
```html
        <div class="div4">Div 4</div>
```
**code css**
```css
.div4{
            background-color: blue;
            clear: right;
            float: none;
     }
```
-----------------------------------------------------------------------------
### MEMBUAT FOLDER BARU DENGAN NAMA lab4_layout, KEMUDIAN BUATLAH FILE BARU DI DALAM NYA DENGAN NAMA **home.html** DAN FILE CSS NYA DENGAN NAMA **style.css**

## 4).BUAT KERANGKA LAYOUT DENGAN SEMANTIC ELEMENT

## CONTOH CODE DAN TAMPILAN DIBROWSER NYA!


**PENJELASAN**

ini adalah web layout dengan menggunakan **semantic element** seperti **header** **footer** dll

**code html**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>Layout Sederhana</h1>
        </header>
        <nav>
            <a href="home.html" class="active">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html">About</a>
            <a href="kontak.html">Kontak</a>
        </nav>
        <section id="hero"></section>
        <section id="wrapper">
            <section id="main"></section>
            <aside id="sidebar"></aside>
        </section>
        <footer>
            <p>© 2022 - Universitas Pelita Bangsa</p>
        </footer>
    </div>
</body>
</html>
```
## 5). MENAMBAHKAN FILE CSS UNTUK MEMBUAT LAYOUT

## CONTOH CODE DAN TAMPILAN DIBROWSER NYA!


**PENJELASAN** 

Setelah membuat dokumen HTML nya kemudian membuat CSS nya dengan menggunakan CSS Eksternal untuk menambahkan gaya dan mengatur ***layout*** nya seperti hasil di atas sudah dengan import font google berikut hasil gambar di atas!

**code html**
```css
/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');

/* Reset CSS */
*{
    margin: 0;
    padding: 0;
}

body{
    line-height: 1;
    font-size: 100%;
    font-family: 'Open Sans',sans-serif;
    color: #5a5a5a;
}
#container{
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}
/* header */
header{
    padding: 20px;
}
header h1{
    margin: 20px 10px;
    color: #b5b5b5;
}
```

## 6).MEMBUAT NAVIGASI

## CONTOH CODE DAN TAMPILAN DIBROWSER NYA!


**PENJELASAN**

Disini ditambahkan CSS pada bagian ***navigasi*** nya seperti contoh gambar di atas.

**code css**
```css
/* navigasi */
nav{
    display: block;
    background-color: #1f5faa;
}
nav a{
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}
nav a.active,
nav a:hover{
    background-color: #2b83ea;
}
```

## 7).MEMBUAT HERO PANEL

## CONTOH CODE DAN TAMPILAN DIBROWSER NYA!


**PENJELASAN**

Disini kita membuat **ID HERO** untuk kemudian ditambahkan beberapa element **html** dan juga **css** seperti contoh gambar di atas!

**code html**
```html
<section id="hero">
            <h1>Hello World</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                pretium ac.</p>
            <a href="home.html" class="btn btn-large">Learn more »</a>
</section>
```
**code css**
```css
/* Hero Panel */
#hero{
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
#hero h1{
    margin-bottom: 20px;
    font-size: 35px;
}
#hero p{
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px;
}
```
## 8). MENGATUR LAYOUT MAIN DAN SIDEBAR

**PENJELASAN**

Code dibawah adalah bagaimana mengatur main dan sidebar dalam bentuk css

**code css**
```css
/* main content */
#wrapper{
    margin: 0;
}
#main{
    float: left;
    width: 640px;
    padding: 20px;
}
/* sidebar area */
#sidebar{
    float: left;
    width: 260px;
    padding: 20px;
}
```

## 9). MEMBUAT SIDEBAR WIDGET

## CONTOH CODE DAN TAMPILAN DIBROWSER NYA!


**PENJELASAN**

Disini dibuat dengan menggunakan **class widget-box** dalam pendeklarasian di css untuk membuat **sidebar widget** seperti gambar di atas dengan ketentuan **float left**
seperti contoh gambar di atas.

**code html**
```html
            <aside id="sidebar">
                <div class="widget-box">
                    <h3 class="title">Widget Header</h3>
                    <ul>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                    </ul>
                </div>
                <div class="widget-box">
                    <h3 class="title">Widget Text</h3>
                    <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
                        arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
                        pharetra est nunc, nec pretium nunc pretium ac.</p>
                </div>
            </aside>
```

**code css**
```css
/* widget */
.widget-box{
    border: 1px solid #eee;
    margin-bottom: 20px;
}
.widget-box .title{
    padding: 10px 16px;
    background-color: #428bca;
    color: #fff;
}
.widget-box ul{
   list-style-type: none;
}
.widget-box li{
    border-bottom: 1px solid #eee;
}
.widget-box li a{
    padding: 10px 16px;
    color: #333;
    display: block;
    text-decoration: none;
}
.widget-box li:hover a{
    background-color: #eee;
}
.widget-box p{
    padding: 15px;
    line-height: 25px;
}
```

## 10). MENGATUR  FOOTER

## CONTOH CODE DAN TAMPILAN DIBROWSER NYA!


**PENJELASAN**

Disini ditambahkan CSS pada bagian **footer** nya seperti contoh gambar di atas.

**code css**
```css
/* footer */
footer{
    clear: both;
    background-color: #1d1d1d;
    padding: 20px;
    color: #eee;
}
```

## 11).MENAMBAHKAN ELEMENT LAINNYA PADA MAIN CONTENT

## CONTOH CODE DAN TAMPILAN DIBROWSER NYA!


**PENJELASAN**

Disini ditambahkan beberapa element HTML dan juga CSS pada bagian **section id main** 

**code html**
```html
<section id="main">
                <div class="row">
                    <div class="box">
                        <img src="https://dummyimage.com/120/db7d25/fff.png" alt="erorr" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
                            euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="erorr" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="erorr" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                </div>
 </section>
```

**code css**
```css
/* box */
.box{
    display: block;
    float: left;
    width:33.333333%;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing:border-box;
    padding: 0 10px;
    text-align: center;
}
.box h3{
    margin: 15px 0;
}
.box p{
    line-height: 20px;
    font-size: 14px;
    margin-bottom: 15px;
}
box img{
    border: 0;
    vertical-align: middle;
}
.image-circle{
    border-radius: 50%;
}
.row{
    margin: 0 -10px;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing: border-box;
}
.row::after, .row::before,
.entry::after, .entry::before{
    content: '';
    display: table;
}
.row::after,
.entry::after{
    clear: both;
}
```

## 12). MENAMBAHKAN CONTENT ARTIKEL PADA MAIN CONTENT

## CONTOH CODE DAN TAMPILAN DI BROWSER NYA!
![content_artikel](img/content_artikel.png)

**PENJELASAN**

Disini ditambahkan beberapa element html dalam membuat content artikel dalam **id main** dan juga ditambahkan gaya pada css,seperti gambar di atas adalah contoh nya.

**code html**
```html
                <hr class="divider">
                <article class="entry">
                    <h2>First featurette heading</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="erorr">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                        elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                        vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                        pretium ac.</p>
                </article>
                <hr class="divider">
                <article class="entry">
                    <h2>First featurette heading</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="erorr" class="right-img">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                        elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                        vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                        pretium ac.</p>
                </article>
```

**code css**
```css
/*  hr divider  */
.divider{
    border: 0;
    border-top: 1px solid #eeeeee;
    margin: 40px 0;
}
/* entry */
.entry{
    margin: 15px 0;
}
.entry h2{
    margin-bottom: 20px;
}
.entry p{
    line-height: 25px;
}
.entry img{
    float: left;
    border-radius: 5px;
    margin-right: 15px;
}
.entry .right-img{
    float: right;
}
```

-------------------------------------------------------------------------------------------------------------
## PERTANYAAN DAN TUGAS!

## 1). TAMBAHKAN LAYOUT UNTUK MENU ABOUT
##     => BUAT SINGLE LAYOUT YANG BERISI DESKRIPSI,PORTOFOLIO,DLL
* Buat file HTML baru dengan nama **about.html**, dan buat single layout yang berisi: deskripsi,portofolio,dll

## CONTOH CODE DAN TAMPILAN BROWSER NYA!
![about](img/about.png)
