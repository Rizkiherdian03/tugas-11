# tugas-11
Dasprog


#!/usr/bin/env python
# coding: utf-8

# In[30]:


def luas_dan_keliling():
    # Program Menghitung Luas dan Keliling
    print
    print("------------------------------------------------")
    print("Program Menghitung Luas dan Keliling")
    print("------------------------------------------------")
    print
    # Pilihan
    while True:
        try:
            print("Luas dan Keliling:")
            print(" 1. Luas Segitiga \n 2. Luas Persegi Panjang \n 3. Keliling Persegi Panjang \n 4. Keliling Lingkaran \n 5. Back \nPilih Salah Satu: ")
            pilih = int(input("Masukan Pilihan Anda: "))
            print()
        except ValueError:
            print("Inputan harus berupa number😑")
            print()
        else:
            if pilih == 1:
                print("Hitung Luas Segitiga")
                print("-------------------------------")
                
                alas = float(input('Masukan alasnya: '))
                tinggi = float(input('Masukan tingginya: '))

                luas = 1/2 * (alas * tinggi)
                print('\nLuasnya =', str(luas))
                print()

            elif pilih == 2:
                print('Hitung Luas Persegi Panjang')
                print("------------------------------")

                panjang = float(input('Masukan panjangnya: '))
                lebar = float(input('Masukan lebarnya: '))

                luas = panjang * lebar
                print('\nLuasnya =', str(luas))
                print()

            elif pilih == 3:
                print('Hitung Keliling Persegi Panjang')
                print("------------------------------")

                panjang = float(input('Masukan panjangnya: '))
                lebar = float(input('Masukan lebarnya: '))

                keliling = 2 * (panjang + lebar)
                print('Kelilingnya =', str(keliling))
                print()

            elif pilih == 4:
                print("Hitung Keliling Lingkaran")
                print("--------------------------------")

                phi = 3.14
                r = float(input("Masukkan panjang jari-jari lingkaran: "))

                keliling = 2 * phi * r
                print('Kelilingnya =', str(keliling))
                print()
            
            elif pilih == 5:
                break

            else:
                print("Error: Inputkan Angka Yang Benar..😑")
                print()
                
def Bayar_Kos(Biaya_Kos = 850000, Keterlambatan = 5, Denda_Keterlambatan = 50000 ):
    Bayar = Biaya_Kos + (Keterlambatan * Denda_Keterlambatan)
    print("Biaya Kos = Rp. 850.000")
    print("Denda_Terlambat = Rp. 50.000 Perhari")
    print("Keterlambatan = 5 Hari")
    print("Jumlah yang harus dibayar adalah: ","Rp.", Bayar)
    print("Harus dibayar yaa😉😊")
    print()
    
while True:
    try:
        userInput = int(input(
            "MENU : \n 1. Menghitung Luas dan Keliling \n 2. Bayar Kos \n 3. Quit\nPilih Nomer: "))
        print()
    except ValueError:
        print("Inputan harus berupa number😑")
        print()
    else:
        if (userInput == 1):
            luas_dan_keliling()
        elif (userInput == 2):
            Bayar_Kos()
        elif (userInput == 3):
            print("Terima Kasih Sudah Pakai Program Saya🤗")
            break
        else:
            print("Pilih Salah Satu Yaa🤨")
            print()


# In[ ]:



