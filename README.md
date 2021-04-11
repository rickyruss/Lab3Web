# Lab3Web
## Langkah-langkah pembuatan:
- Pertama,Membuat Tag html dasar dengan dinamai file lab 3 list,dengan bertujuan menggunakan list sebagai berikut. Lalu buatlah nama order list ada 3.
![q1](https://user-images.githubusercontent.com/56240498/114295468-a578d780-9acf-11eb-8bb9-c156b469d9ed.jpg)
- Kedua,Membuat kata unordered list pada section berikut.
![q2](https://user-images.githubusercontent.com/56240498/114295470-a7db3180-9acf-11eb-8ae0-36c59c06285d.jpg)
- Lalu membuat Deskripsi list pada bagian berikut.
![q3](https://user-images.githubusercontent.com/56240498/114295472-a9a4f500-9acf-11eb-91cb-c71e4b624473.jpg)
- Lalu membuat file baru yang isinya terdapat tabel pada gambar berikut.
![q4](https://user-images.githubusercontent.com/56240498/114295474-ab6eb880-9acf-11eb-91ae-e34b6ff8c8c1.jpg)
- Menambahkan style rospawn agar tulisan teknik menjadi 1 pada tabel berikut.
![q5](https://user-images.githubusercontent.com/56240498/114295481-b32e5d00-9acf-11eb-87d7-86cbb6f260b2.jpg)
- Lalu membuat form tabel pada modul yang suda diajarkan.
![q6](https://user-images.githubusercontent.com/56240498/114295483-b45f8a00-9acf-11eb-890b-49ba9776ebcd.jpg)
## Pertanyaan dan Tugas
1. Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.
![q7](https://user-images.githubusercontent.com/56240498/114295465-a27de700-9acf-11eb-874b-2eaeae45eb1b.jpg)
# Berikut Codinganya:
## Dropdown.html
```
<html>
<head>
    <title>Drop-down Menu</title>
    <link rel="stylesheet" href="Style.css">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
<body>
<div class="menu-bar">
<ul>
<li class="active"><a href="#"><i class="fa fa-home"></i>Home</a>
</li>
<li><a href="#"><i class="fa fa-user"></i>About us</a>
    <div class="sub-menu-1">
        <ul>
            <li><a href="#">Mission</a></li>
            <li><a href="#">Vision</a></li>
            <li><a href="#">Team</a></li>
        </ul>
    </div>
</li>
<li><a href="#"><i class="fa fa-clone"></i>Services</a>
<div class="sub-menu-1">
<ul>
<li><a href="#">Web Design</a></li>
<li class="hover-me"><a href="#">Marketing</a><i class="fa fa-angle-right"></i>
    <div class="sub-menu-2">
        <ul>
            <li><a href="#">SEO</a></li>
            <li><a href="#">Social Media</a></li>
            <li><a href="#">Email Marketing</a></li>
        </ul>
    </div>
</li>
<li><a href="#">Mobile app</a><i class="fa fa-angle-right"> </i></li>
</ul>
</div>
</li>
<li><a href="#"><i class="fa fa-users"></i>Clients</a></li>
<li><a href="#"><i class="fa fa-angellist"></i>Investers</a></li>
<li><a href="#"><i class="fa fa-inr"></i>pricing</a></li>
<li><a href="#"><i class="fa fa-edit"></i>Training</a></li>
<li><a href="#"><i class="fa fa-phone"></i>Contact</a></li>
</ul>
</div>
</body>
</html>
```
## Style.css
```
*
{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
body
{
    background-image: url(alam.jpg);
    background-size: cover;
    background-position: center;

    font-family: sans-serif;
}
.menu-bar
{
    background: rgb( 0,100,0);
    text-align: center;
}
.menu-bar ul
{
    display: inline-flex;
    list-style: none;
    color: #fff;
}
.menu-bar ul li
{
    width: 120px;
    margin: 15px;
    padding: 15px;

}
.menu-bar ul li a
{
    text-decoration: none;
    color: #fff;
}
.active, .menu-bar ul li:hover
{
    background: #2bad0d;
    border-radius: 3px;

}
.menu-bar .fa
{
    margin-right: 8px;
}

.sub-menu-1
{
    display: none;
}
.menu-bar ul li:hover .sub-menu-1
{
    display: block;
    position: absolute;
    background: rgb( 0,100,0);
    margin-top: 15px;
    margin-left: -15px;
}
.menu-bar ul li:hover .sub-menu-1 ul
{
    display: block;
    margin: 10px;
}
.menu-bar ul li:hover .sub-menu-1 ul li
{
    width: 150 px;
    padding: 10px;
    border-bottom: 1px dotted #fff;
    background: transparent;
    border-radius: 0;
    text-align: left;
}
.menu-bar ul li:hover .sub-menu-1 ul li:last-child
{
    border-bottom: none;
}
.menu-bar ul li:hover .sub-menu-1 ul li a:hover
{
    color: #b2ff00;
}

.fa-angle-right
{
    float: right;
}
.sub-menu-2
{
    display: none;
}
.hover-me:hover .sub-menu-2
{
    position: absolute;
    display: block;
    margin-top: -40px;
    margin-left: 140px;
    background: rgba(0,100,0);
}
```
