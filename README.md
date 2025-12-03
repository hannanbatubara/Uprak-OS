# Uprak-OS
<img width="641" height="780" alt="image" src="https://github.com/user-attachments/assets/485bdf7d-c0cb-47bd-b74d-2084f0a46da6" />
<img width="625" height="763" alt="image" src="https://github.com/user-attachments/assets/1d2422e5-d408-411a-936c-2bae1206df11" />
<img width="514" height="688" alt="image" src="https://github.com/user-attachments/assets/a7244eb5-4098-4ec1-8d3c-3d741ee41af7" />
<img width="532" height="835" alt="image" src="https://github.com/user-attachments/assets/d25bb155-8f77-406a-9cdf-5fcd01b8b3b2" />
<img width="484" height="691" alt="image" src="https://github.com/user-attachments/assets/0a1e596b-6356-4da2-934c-2402e6bdcf3d" />
<img width="835" height="247" alt="image" src="https://github.com/user-attachments/assets/628cea4f-0953-4415-bf29-62aa10ede2b0" />
<img width="506" height="581" alt="image" src="https://github.com/user-attachments/assets/31c0574b-60ff-409e-ba49-41a552f7d90a" />
<img width="509" height="721" alt="image" src="https://github.com/user-attachments/assets/114395f1-904a-4889-9f8c-87d028d2d18b" />
<img width="481" height="331" alt="image" src="https://github.com/user-attachments/assets/62ea56f6-3dc7-44ee-80ec-6b2a7c9e40fa" />
<img width="795" height="587" alt="image" src="https://github.com/user-attachments/assets/0284d6aa-4125-4531-82ec-f558b2275848" />
# pindah ke direktori home anda
cd ~

# buat satu folder kosong 'test'
mkdir test

# masuk ke direktori 'test'
cd test

# tampilkan path direktori saat ini
pwd

# buat file kosong bernama 'empty.txt'
touch empty.txt

# copy file '/etc/timezone' ke direktori ini
cp /etc/timezone .

# ubah nama file 'timezone' menjadi 'tz.txt'
mv timezone tz.txt

# list isi direktori ini
ls -l

# pindah ke direktori parent
cd ..

# hapus direktori 'test' seisinya
rm -r test

# temukan file dengan nama 'fdisk' memakai `locate`
locate fdisk

# temukan file dengan nama 'fdisk' memakai `find`
find / -name "fdisk" 2>/dev/null

# temukan file pada home anda yang ukurannya > 200 MB
find ~ -size +200M 2>/dev/null

# temukan file pada home anda yang diubah < 3 hari
find ~ -mtime -3 2>/dev/null

# temukan file pada home anda yang diakses > 30 hari
find ~ -atime +30 2>/dev/null

# tampilkan 5 baris pertama keluaran perintah `last`
last | head -n 5

# tampilkan dua baris terakhir file '/etc/passwd'
tail -n 2 /etc/passwd

# cari file di '/usr/include' yang memuat kata 'sem_post'
grep -R "sem_post" /usr/include 2>/dev/null

# tampilkan kolom 1 dan 5 dari file '/etc/passwd'
cut -d: -f1,5 /etc/passwd

# tampilkan isi file '/etc/motd' dalam huruf kapital
tr 'a-z' 'A-Z' < /etc/motd

# jalankan `cat /dev/random > rand.txt` di background
cat /dev/random > rand.txt &

# tampilkan daftar job
jobs

# kirim sinyal STOP ke job tersebut
kill -STOP %1

# lanjutkan job tersebut di background
kill -CONT %1

# kirim sinyal TERM ke job tersebut
kill -TERM %1
