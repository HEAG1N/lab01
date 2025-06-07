IWNO1: Server virtual

Realizat de: Balea Artiom I2301

Scop

Am descarcat distributivul Debian pentru servere pentru arhitectura x64 (fără interfață grafică) și sistemul de virtualizare (hypervizor) QEMU. Executare

Am creat directorul lab01. În acest director am creat directorul dvd și fișierul readme.md. În directorul dvd am plasat imaginea ISO a distributivului Debian.

În consolă am creat în directorul lab01 imaginea discului pentru mașina virtuală de dimensiune 8 GB și format qcow2, folosind utilitarul qemu-img:

![image](https://github.com/user-attachments/assets/62e7dbcf-183e-49df-bf3a-2bedf0871e4e)

Am instalat SO Debian pe mașina virtuală. Pentru aceasta am executat comanda:

![image](https://github.com/user-attachments/assets/760d6570-6e31-4dc7-90ef-a1c739d266dc)

![image](https://github.com/user-attachments/assets/868fec43-fa3f-4729-bdb6-ad7b350e1c65)

Repornim mașina virtuală. Pentru a reporni mașina virtuală, am executat comanda:

![image](https://github.com/user-attachments/assets/8cd9d1fd-3c62-4414-a2b1-212a0a69a425)

Am instalat LAMP în mașina virtuală. Pentru aceasta, am schimbat profilul utilizatorului pe superutilizator. Descarcam SGBD PhpMyAdmin si CMS Drupal. Dezarhivam fișierele descărcate:

<img width="854" src="https://github.com/user-attachments/assets/dd5ef4b5-3871-42f1-a4ea-5e45f7f2a6bd" />

Creeam din linia de comandă baza de date drupal_db și utilizatorul bazei de date:

<img width="563" src="https://github.com/user-attachments/assets/49987e1a-1f72-4664-bb5c-042c9883b470" />

În directorul /etc/apache2/sites-available am creat fișierul 01-phpmyadmin.conf , cu următorul conținut:

<img width="850"  src="https://github.com/user-attachments/assets/8c37f59f-382d-4611-b307-f0ed55cc18d7" />

În directorul /etc/apache2/sites-available creați fișierul 02-drupal.conf

<img width="808" src="https://github.com/user-attachments/assets/71e01c3c-3d6e-40c0-b801-acefc589ecf2" />

Pentru a activa configurațiile, am executat comenzile:

<img width="853" src="https://github.com/user-attachments/assets/c62b49e7-1c8a-4f86-8d63-6ccc031c6485" />

Am repornit Apache HTTP Server:

<img width="419" src="https://github.com/user-attachments/assets/900f285d-4278-4f09-a5dd-83e52613466c" />


