# Introduction
  Penggunaan Azure SQL in Virtual Machine biasanya digunakan untuk memudahkan migrasi dari SQL yang berada di On-premise untuk dipindahkan
  ke cloud. Azure SQL in VM digunakan untuk menyesuaikan dengan aplikasi vendor thirdparty yang membutuhkan OS untuk bisa running.  
  
##  Alasan IAAS sebagai pilihan pemasangan SQL Server in Azure
    - Older Version of SQL Server - jika aplikasi membutuhkan version SQL Server tertentu untuk mendukung App Vendor lain
    yang berjalan ddalam sebuah VM adalah pilihan terbaik menggunakan SQL Server in VM
    
    - Menggunakan other SQL Server Services - ketika Analysis Services and untuk Extent integration services(menggunakan Azure data Factory)
    yang tersedia di PAAS, bayak user memaksimalkan license dengan menjalankan SQL Server Analysis Service, Integration Service, or Reporting Service pada 
    pada VM yang sama
    
    - General Application Incompatibility -  ini adalah alasan mencangkup semua. sebagai contoh, Azure SQL Database tidak mendukung **Cross-database query**
    ketika managed instance dilakukan. beberapa aplikasi mungkin menggunakan layanan tambahan sebagai co-located dengan
    database instace yang tidak kompatibel dengan PAAS.
