# perhitungan-sederhana

Membuat penjumlahan berdasarkan data dari dictionary

Kali ini kita akan membuat sebuah perhitungan sederhana dimana data yang akan hitung tersimpan didalam sebuah dictionary. Kita akan mengakses datanya berdasarkan key

Langkah-langkah

	

1. Kita membutuh beberapa variabel yang akan di isi nantinya dengan beberapa data yang dikumpulkan dalam satu dictionary
  
        sepatu = { "nama" : "Sepatu Niko", "harga": 150000, "diskon": 30000 }
	
        baju = { "nama" : "Baju Unikloh", "harga": 80000, "diskon": 8000 }
	
        celana = { "nama" : "Celana Lepis", "harga": 200000, "diskon": 60000 }
   
   Terdapat 3 variabel yang berisi dictionary pada kasus kali ini (sepatu, baju, celana)
   
   Seperti yang kita ketahui bahwa dalam dictionary memiliki yang namanya 'key' ditandai dengan sebuah string yang terletak sebelum titik dua (:), contohnya pada variabel diatas key nya adalah "nama", "harga", "diskon"
	
2. Lalu kita membuat 3 variabel baru yang nantinya akan mencari harga setelah diskon  
	
        harga_sepatu = sepatu["harga"] - sepatu["diskon"]
	      
        harga_baju = baju["harga"] - baju["diskon"]
	      
        harga_celana = celana["harga"] - celana["diskon"]
        
    Tiga variabel ini menampung hasil pengurangan harga barang (sepatu, baju, celana) yang dikalikan dengna diskon masing-masingnya.
  
    Maksud dari sepatu["harga"] ini adalah mengambil data dari dictionary dengan key "harga" yang artinya mengambil angka 150000 dikurang data dari key "diskon" yang dimana berisi angka 30000
  
    Dan begitu seterusnya pada harga_baju dan harga_celana
    
3. Terakhir kita buat variabel total_harga, yang akan menambahkan variabel harga_sepatu, harga_baju, harga_celana tadi yang telah kita buat. Kemudian dikali dengan pajak 10%, kita buat menjadi 1.1

        total_harga = (harga_sepatu + harga_baju + harga_celana) * 1.1
        
   Kita memasukkan variabel penambahan ke dalam sebuah tanda kurung agar proses yang dilakukan terlebih dahulu adalah penambahan bukan perkalian. Ini merupakan sifat dasar dari perhitungan matematika
   
   Kemudian print variabel total_harga 
    
        print(total_harga)
