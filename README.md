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
