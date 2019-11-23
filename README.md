:octocat: PROGRAM MENAMBAHKAN DATA KEDALAM SEBUAH LIST :octocat:

FLOWCHART PROGRAM :

![flowchartlist](https://user-images.githubusercontent.com/57025775/69469022-4377df00-0dc1-11ea-8992-4fcc6ab00be0.jpg)

ALUR ALGORITMA PROGRAM :

1.	Buat list kosong yang nantinya akan di isi berdasarkan data yang akan kita input. 
2.	Lalu buat perintah input berupa Nama, Nim, Nilai tugas, Nilai UTS, dan Nilai UAS. nilai input ini berfungsi untuk menampilkan data nilai akhir. Dimana Nilai akhir di ambil dari perhitungan 3 komponen nilai (tugas : 30%, uts : 35%, uas : 35%) 
3.	Gunakan perintah "append" untuk memasukan data yang akan kita buat ke dalam list kosong yang sudah di buat di awal. 
4. Tampilkan pertanyaan untuk menambah data (ya/tidak), apabila memilih “ya” maka akan muncul perintah untuk memasukan data nama, nim, nilai tugas, nilai uts dan nilai uas  , dan apabila memilih “tidak” program akan berhenti dan menampilkan data yang telah dimasukan beserta nilai akhir.
5.	Buatlah perulangan "for" dan masukan list yang sudah terisi tadi pada perintah "print" agar semua data yang masuk bisa di munculkan pada program


CODE PROGRAM :

    NML =[]     #nama mahasiswa
    NIML =[]    #nim
    NTL =[]     #nilai tugas
    NUTSL =[]   #nilai uts
    NUASL =[]   #nilai uas
    NAML=[]     #nilai akhir

    print(" PROGRAM MENAMBAHKAN DATA DALAM LIST")
    print("")

    jawab ="ya"
    while jawab == "ya" :
        NM=input("Nama  :")
        NIM=input("NIM :")
        NTUGAS=float(input("Nilai Tugas:"))
        NUTS=float(input("Nilai UTS:"))
        NUAS=float(input("Nilai UAS:"))
        nilai=float(NTUGAS)*30/100 + (NUTS)*35/100 + (NUAS)*35/100
        print("")

        NML.append(NM)
        NIML.append(NIM)
        NTL.append(NTUGAS)
        NUTSL.append(NUTS)
        NUASL.append(NUAS)
        NAML.append(nilai)

    lagi = input("Tambah Data [ya/tidak]? :")
    print("")
    if lagi =="tidak":
        break

    print ("                           DAFTAR MAHASISWA                           ")
    print (70*'=')
    print ("| NO |    Nama  |      NIM     |  Tugas |  UTS   |   UAS   |  Akhir  |")
    print (70*'=')

    for n in range (len(NML)):
        print(' ',n+1,   ' |   ',NML[n],  '|  ',NIML[n],' | ',NTL[n],' | ',NUTSL[n],' |  ',NUASL[n],' | ',NAML[n],' |' )
    print ("")
    print (70*'=')
    
CONTOH HASIL PROGRAM :
![listtambah](https://user-images.githubusercontent.com/57025775/69469028-4d014700-0dc1-11ea-9f2e-2f73533cf60e.jpg)

Demikian program untuk menambahkan data ke dalam list , Semoga bermanfaat :octocat: 
