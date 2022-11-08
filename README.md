#### Nama : Amanda Puspa Negara
#### Nim : 312210129
#### Kelas : TI.22.A1

KONDISI DAN PERULANGAN

Lab 2 Struktur Kondisi

Latihan 1

• Buat program sederhana dengan input 2 buah bilangan, kemudian tentukan bilangan terbesar dari kedua bilangan tersebut menggunakan statement if!

Langkah - langkah

1. Buat programnya terlebih dahulu seperti gambar di bawah ini
![Screenshot (71)1](https://user-images.githubusercontent.com/115678845/200473277-885c691a-e46e-4835-9edf-8f3758e9d6e9.png)

        a = (input("masukkan angka a: "))
        b = (input("masukkan angka b: "))
        if a >= b:
            print(a, "bilangan terbesar ")
            print(b, "bilangan terkecil ")
          
  2. Hasil Run
  
  ![Screenshot (71)2](https://user-images.githubusercontent.com/115678845/200473521-8956ef6c-b6ef-403d-8adf-7c4f19fcab77.png)

Latihan 2

• Buat program untuk mengurutkan data berdasarkan input sejumlah data (minimal 3 variable input atau lebih), kemudian tampilkan hasilnya secara berurutan mulai dari data terkecil.

Langkah - langkah

1. Buat programnya terlebih dahulu seperti gambar di bawah ini

![Screenshot (72)](https://user-images.githubusercontent.com/115678845/200473920-90f0323f-747d-4503-8d04-953b3b27756c.png)

        print("_____Mengurutkan bilangan dari yang terkecil ke yang terbesar_____")
        print("Masukan 3 bilangan yang akan diurutkan:")
        a = int(input("masukkan bilangan 1 = "))
        b = int(input("masukkan bilangan 2 = "))
        c = int(input("masukkan bilangan 3 = "))

        if a < b and a < c:
            if b < c:
                print(a, b, c)
            else:
                print(a, c, b)
        elif b < a and b < c:
            if a < c:
                print(b, a, c)
            else:
                print(b, c, a)
        else:
            if a < b:
                print(c, a, b)
            else:
                print(c, b, a)

2. Hasil run

![Screenshot (73)1](https://user-images.githubusercontent.com/115678845/200474315-539149d4-9329-4ef3-b558-e2c9205006a8.png)

Lab 3 Perulangan

Latihan 1

• Buat program dengan perulangan bertingkat (nested) for yang menghasilkan output sebagai berikut:

Langkah - langkah

1. Buat programnya terlebih dahulu seperti gambar di bawah ini

![Screenshot (74)1](https://user-images.githubusercontent.com/115678845/200474945-fe8f2848-36cd-4ca3-aff4-45c587c641d6.png)

      for i in range(0,10):
          print()
          print(i, end="\t")
          for j in range(1,10):
              print(i+j,end="\t")
              
2. Hasil run

![Screenshot (75)1](https://user-images.githubusercontent.com/115678845/200475146-b01e9c97-e70c-40c5-b7f2-ccc7ceee73f9.png)

Latihan 2

• Tampilkan n bilangan acak yang lebih kecil dari 0.5.

• nilai n diisi pada saat runtime

• anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya

Langkah - langkah

1. Buatlah programnya terlebih dahulu seperti gambar dibawah ini

![Screenshot (76)1](https://user-images.githubusercontent.com/115678845/200475709-e1548ca4-affa-4e2d-977d-7a1e487c06aa.png)

        from random import random

        n = int(input("Masukan Beberapa perulangan : "))
        while n == n:
            break
        for i in range(n):
            bil = random() % 0.5
            print("Perulangan ke : ", bil)
            
2. Hasil run

![Screenshot (76)2](https://user-images.githubusercontent.com/115678845/200475934-1c96a8ce-61e5-4f03-a322-cbd529047715.png)

MODUL PRAKTIKUM 2 DAN 3

Labpy02 dan Labpy03

Labpy02

• Buat program sederhana dengan input tiga buah bilangan, dari ketiga bilangan tersebut tampilkan bilangan terbesarnya. Gunakan statement if.

Langkah - langkah

1. Buatlah flowchart dari mencari angka terbesar dari 3 bilangan seperti gambar dibawah ini

![200346173-1bd4dc03-340d-4bcb-985f-6777380dce97](https://user-images.githubusercontent.com/115678845/200476548-e3c66404-05cc-4cfe-a74d-95bea8d20434.png)

2. Buatlah program codenya seperti gambar dibawah ini

![Screenshot (77)](https://user-images.githubusercontent.com/115678845/200476882-c3ed4196-5f05-4e3a-9903-3269f026feee.png)

        a, b, c = (
              int(input('Masukkan nilai a: ')),
              int(input('Masukkan nilai b: ')),
              int(input('Masukkan nilai c: '))
          )
          if a > b and a > c:
              print('A yang terbesar')
          elif b > a and b > c:
              print('B yang terbesar')
          else:
              print('C yang terbesar')
              
2. Hasil dari run

![Screenshot (78)1](https://user-images.githubusercontent.com/115678845/200477347-14d9df28-211a-41ed-9064-575ec88c22e9.png)

Labpy03

Latihan 1

Flowchart dari latihan 1

![200347193-02e0f924-4055-4a30-8bd3-a4fad535dd5f](https://user-images.githubusercontent.com/115678845/200477455-145270d5-0d27-4a66-ac7d-7535b3db9e10.png)

Algoritma dari latihan 1

Menampilkan n bilangan acak yang lebih kecil dari 0,5, nilai n diisi pada saat runtime.

1.Memasukan/ import fungsi RANDOM terlebih dahulu

2.Deklarasi integer , masukkan jumlah n :

3.Memasukan deskripsi kombinasi for untuk menyelesaikannya.

4.Memasukan nilai jumlah (n) : 5

5.Mencetak data ke 1 sampai 5 dengan hasil nilai kurang dari 0,5.

6.Selesai

Langkah - langkah

1. Buat program codenya seperti gambar dibawah ini

![Screenshot (81)1](https://user-images.githubusercontent.com/115678845/200478113-1060fa84-77ad-4494-9ff8-9a486ee35ac1.png)

        print("bilangan acak yang lebih kecil dari o.5")
        import random

        n = int(input("masukan nilai:"))
        a = 0
        for c in range(n):
            a += 1
            b = random.uniform(.0, .5)
            print("data ke:", a, "==>", b)

        print("selesai")
        
2. Hasil run

![Screenshot (81)2](https://user-images.githubusercontent.com/115678845/200478274-8a17db97-859b-4dc3-a1e2-27e4f2d2bb07.png)

Latihan 2

Flowchart dari latihan 2
![200348255-0af9262f-70eb-47dd-aa24-cd119827c0d2](https://user-images.githubusercontent.com/115678845/200478421-663ec5d4-0cda-492a-9dd1-b6b381f23438.png)

Algoritma latihan 2

Membuat program untuk menampilkan bilangan terbesar dari n buah data yang diinputkan.Masukkan angka 0 untuk berhenti

1.Mulai

2.Mencetak "latihan 2"

3.Mencetak "menampilkan bilangan, berhenti ketika bilangan 0, menampilkan bilangan terbesar"

4.integer max = 0

5.Menggunakan fungsi perulangan while true, hingga menampilkan perulangan sampai batas tertentu.

6.Memasukan bilangan integer pada "a"

7.Menggunakan fungsi if jika max kurang dari nilai a, maka max sama dengan a

8.Mengunakan fungsi if jika nilai a adalah 0 maka fungsi break artinya perulangan berhenti jika menulis nilai 0.

9.Mencetak nilai paling terbesarv setelah break, sehingga menampilkan nilai terbesar diantara bilangan tersebut dalam perulangan.

10.Selesai

Langkah - langkah

1. Buatlah program code seperti gambar dibawah ini

![Screenshot (82)1](https://user-images.githubusercontent.com/115678845/200479064-5f526367-f057-4911-a7b5-f25ca3dfc800.png)

      print("menampilkan bilangan, berhenti ketika bilangan 0, dan menampilkan bilangan terbesar")

      max = 0
      while True:
          angka = int(input("masukan bilangan : "))
          if max < angka:
              max = angka
          if angka == 0:
              break
      print("bilangan terbesarnya adalah = ", max)
      print("selesai")

2. Hasil run

![Screenshot (82)2](https://user-images.githubusercontent.com/115678845/200479357-72080566-ad61-48b3-8ece-9299a1de64b6.png)

Program 1

Flowchart dari program 1

![200349134-bdde8962-47de-401f-b0b8-e91ff808b329](https://user-images.githubusercontent.com/115678845/200479441-b56cb6d8-f913-4e38-a3b5-8ac4f5cff464.png)
Algoritma dari program 1

1.Mulai

2.Mencetak latihan1

3.Mencetak "Program menghitung laba dengan modal awal 100 juta"

4.Membuat Note

5.Mencetak Bulan pertama dan kedua = 0%

6.Mencetak bulan ke 3 = 1%

7.Mencetak bulan ke 5 = 5%

8.Mencetak bulan ke 8 = 2%

9.integer a = 100.000.000( modal awal)

10.Menggunakan fungsi looping for pada nilai x 1-9 untuk menampilkan bulan 1 sampai bulan 8.

11.Menggunakan fungsi if, untuk menghitung laba bulan 1 sampai 8

12.bulan pertama dan kedua laba adalah 0

13.bulan ke 3 dan ke 4 mendapat laba 1% sehingga modal di kali 1% = keuntungan

14.bulan ke 5 mendapatkan laba 5%, sehingga modal dikali 5% = keuntungan

15.Bulan ke 8 mmendapatkan laba 2% sehingga keuntungan menurun dari bulan sebelumnya, modal dikali 2% = keuntungan.

16.Menghitung jumlah total laba dengan menjumlah keuntungan dari bulan ke 1 sampai bulan 8, hasilnya adalah total keuntungan yang didapat.

17.Selesai

Langkah - langkah

1. Buatlah program codenya seperti gambar dibawah ini

![Screenshot (83)1](https://user-images.githubusercontent.com/115678845/200479751-a8ae41b2-1886-4f68-b45d-a810435c3887.png)

        x = 100000000
          sum = 0
          y = 0
          lb = [int(0), int(0), int(x) * .1, int(x) * .1, int(x) * .5, int(x) * .5, int(x) * .5, int(x) * .2]
          print("modal awal seorang pengusaha :', x")
          for i in lb:
              sum = sum + i
              y += 1
              print("#laba bulan ke - ", y, "sebesar :", i)

              print("  TOTAL LABA YANG DIDAPAT ADALAH :", sum)
              
2. Hasil run

![Screenshot (84)1](https://user-images.githubusercontent.com/115678845/200479889-9a1d7b9d-3da1-4ff4-8b39-e15a265ab978.png)

TERIMA KASIH.
