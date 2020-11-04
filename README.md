# Penjelasan Praktikum Lab 1 Pertemuan 6

# String format

String formatting atau pemformatan string memungkinkan kita menyuntikkan item kedalam string daripada kita mencoba menggabungkan string menggunakan koma atau string concatenation.

# 1. **String format 1**
Pada syntax / source code string format 1 akan menampilkan output berupa 2 outputan.
Yang pertama (sebelah kiri) akan menampilkan angka urut dari angka 0 hingga 10, sedangkan sebelah kanan akan menampilkan Oprasi Aritmatika Pangkat.
Dengan ketentuan sebagau berikut, oprasi pangkat dengan angka kiri sebagai pokok (Rumus : ** [Bintang dua]) 

# Penjelasan Praktikum Lab 2 Pertemuan 6

## Lab 2
Pada lab 2 kita mencoba untuk mengoperasikan operator, contoh:
```python
1. a = input("Masukkan nilai a: ")
2. b = input("Masukkan nilai b: ")
// Langkah 1 dan 2 nanti akan meminta kita untuk memasukkan nilai kepada variable a dan b.
3. print("Variable a= ", a)
4. print("Variable b= ", b)
// Langkah 3 dan 4 akan menuliskan ulang nilai yang telah kita masukkan tadi.
5. print("Hasil penggabungan {1}&{0}= %d".format(a,b) %(a+b))
// Langkah 5 akan menggabungkan variable a dan b, tetapi pada tahap ini akan terjadi error karena tipe data pada variable adalah string sedangkan yang diminta adalah integer, maka kita ubah %d menjadi %s. Lalu karena {1} adalah variable b dan {0} adalah variable a (b, a), maka diubah menjadi {0}&{1} agar tidak terbalik dan sesuai dengan format yang akan digabungkan.
6. a=int(a)
7. b=int(b)
// Langkah 6 dan 7 akan mengkonversikan tipe data variable a dan b, dari yang tadinya str menjadi int.
8. print("Hasil penjumlahan {1}+{0}=%d".format(a,b) %(a+b))
// Langkah 8 akan menjumlahkan nilai variable a dan b, dan sebaiknya {1}+{0} diubah menjadi {0}+{1}
9. print("Hasil pembagian {1}/{0}=%d".format(a,b) %(a/b))
// Langkah 9 akan melakukan pembagian nilai variable a dengan b, ubah {1}/{0} menjadi {0}/{1} agar nilai yang dibagi sesuai dengan hasilnya. Gunakan '%f' atau '%s' apabila hasilnya adalah angka desimal.
