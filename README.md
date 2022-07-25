# Men-deploy React.js ke Hosting
## Siapkan project
Sebelum melakukan deploy, siapkan project terlebih dahulu

## Akses SSH
Akses SSH dengan menggunakan terminal dengan command


```
ssh username@alamat_server
``` 

untuk melakukan koneksi

## Melakukan clone pada folder /var/www/html/
Setelah mengakses ssh, masuk pada folder yang dituju dengan command
```
cd /var/www/html/
```
Kemudian, lakukan clone dengan menggunakan command
```
sudo git clone URL-git-repo
```

## Masuk ke folder repo yang telah dilakukan clone
Setelah melakukan clone project pada folder. Lalu, masuk ke dalam folder yang telah di clone dengan menggunakan command
```
cd nama-folder/
```


kemudian, melakukan install dengan command
```
sudo npm install
```

kemudian, run project dengan command
```
sudo npm start
```
```
sudo npm run build
```

## Masuk pada file project
Kemudian, masuk pada file project yang telah di build dengan command:
```
cd nama-folder/
```

## Menjalankan project dengan PM2
Untuk menjalankan project menggunakan PM2 dapat dilakukan dengan command berikut:
```
pm2 serve build/port --name "nama project" --spa
```

Pastikan nomor port berbeda dengan project lainnya.

## Melihat project yang sedang berjalan
Untuk melihat project yang sedang berjalan dapat menggunakan command sebagai berikut:
```
pm2 list
```

## Membuat server blok
Untuk membuat server blok dapat menggunakan command:
``` cd/etc/nginx/conf.d/
```

## Menjalankan server blok
Untuk menjalankan server blok dapat menggunakan command:
```
sudo cp nama_server_blok nama_server_blok_baru
sudo nano nama_server_blok
sudo mv nama_server_blok nama_server_blok_baru
sudo systemctl reload nginx
sudo systemctl restart nginx
```
