![Faris](screenshot/faris.jpg)</p>

## Program Menu Bilangan ganjil, Bilangan Genap dan Bilangan Bulat</p> </br>

1. Source Code Program: </p></br>
``` dart

import 'dart:io';

void main() {

  print('Masukkan Nama Anda:');
  String nama = stdin.readLineSync()!;

  print('Selamat Datang $nama di Sistem Bilangan... ');
  print('===========================================');
  bool selesai = false;

  while (!selesai) {
    print('MENU PROGRAM');
    print('============');
    print('Silakan Anda Pilih:');
    print('1. Bilangan Genap');
    print('2. Bilangan Ganjil');
    print('3. Bilangan Bulat');
    print('4. Keluar');

    String input = stdin.readLineSync()!;
    int opsi = int.parse(input);

    switch (opsi) {
      case 1:
        cekBilanganGenap();
        break;
      case 2:
        cekBilanganGanjil();
        break;
      case 3:
        cekBilanganBulat();
        break;
      case 4:
        selesai = true;
        print('Terima kasih Telah Memakai Aplikasi Ini');
        print('Devoloper Faris Syahluthfi');
        break;
      default:
        print('Opsi tidak valid. Silakan pilih opsi yang benar.');
        break;
    }
    print('\n');
  }
}

void cekBilanganGenap() {
  print('Masukkan sebuah angka:');
  int angka = int.parse(stdin.readLineSync()!);

  if (angka % 2 == 0) {
    print('$angka adalah bilangan genap.');
  } else {
    print('$angka bukan bilangan genap.');
  }
}

void cekBilanganGanjil() {
  print('Masukkan sebuah angka:');
  int angka = int.parse(stdin.readLineSync()!);

  if (angka % 2 != 0) {
    print('$angka adalah bilangan ganjil.');
  } else {
    print('$angka bukan bilangan ganjil.');
  }
}

void cekBilanganBulat() {
  print('Masukkan sebuah angka:');
  String input = stdin.readLineSync()!;
  double angka = double.parse(input);

  if (angka % 1 == 0) {
    print('$angka adalah bilangan bulat.');
  } else {
    print('$angka bukan bilangan bulat.');
  }
}


```

2. Penjelasan Code Programnya: </p></br>