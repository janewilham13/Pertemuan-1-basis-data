1. Login Users & Password PSQL
   
   ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/efb5fcfb-e5e3-4870-b5ba-6a08ebc17f00)
   
2. Buat Database bisa menggunakan command : CREATE DATABASE polban;

   ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/2e5f0280-c6d5-45ca-8b47-dd4bdef05d4f)

   -  Cek database menggunakan command : \list
     
     ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/00419714-2f1e-491a-bb69-9330afca59fa)

4. Masuk ke database yang telah dibuat :  \connect polban

   ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/7511a0d3-7937-44b0-a584-ad0c4085be50)

5.   Membuat Table
   - Buat  terlebih dahulu data type gender (L/P) dengan command : CREATE TYPE gender AS ENUM (‘L’, ‘P’);
     
     ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/4201b7fb-3ff4-4f45-bd62-9a0199402c66)

   - Membuat table denggan command  : (nomor induk mahasiswa, nama, gender, alamat, kota asal, tanggal lahir,tahun masuk, nomor handphone) dengan command : CREATE TABLE mahasiswa (nomor_induk_mahasiswa int PRIMARY KEY, nama varchar(50), gender gender, alamat varchar(50), kota_asal varchar(20), tanggal_lahir date, tahun_masuk int, nomor_handphone int8);

      ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/85502da0-0c50-4c5b-997c-716232277c92)

6. Cek Table
   - cek tabel kosong yang telah dibuat : SELECT * FROM mahasiswa;
     
     ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/a12b7d1f-b154-4963-8250-10cc8d690623)
     
   - cek tabel database : \dt

     ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/c1eea888-d517-4fa8-b7e5-42ebf6d2f724)
    
8. Buat isi table : INSERT INTO mahasiswa (nomor_induk_mahasiswa, nama, gender, alamat, kota_asal, tanggal_lahir, tahun_masuk, nomor_handphone) VALUES (221331046,  'Jane Wilham Aziz Fadhillah', 'L', 'Jl.Sukagalih', 'Bandung', '13-03-2004', 2022, 6285864524634);

Lalu masukkan data absen seperti command tersebut.
   ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/7a31afb3-1f80-4b57-8b67-d0de99999dfe)

9. Cek table yang telah dibuat : SELECT * FROM mahasiswa;

   ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/60730f2f-1527-4f0d-8a28-3bc0bbdb39dc)

11. Tampilan di DBeaver

    ![image](https://github.com/janewilham13/Pertemuan-1-basis-data/assets/148308561/6916bc59-a040-470d-b2d6-abd1b0b4670e)


    




   
     

