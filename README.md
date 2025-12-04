<img width="702" height="921" alt="image" src="https://github.com/user-attachments/assets/9fc37ec7-3200-4e0b-bc35-690afb50d25c" />
<img width="703" height="592" alt="image" src="https://github.com/user-attachments/assets/cbb04eb1-df11-43bb-9a72-3f3c35f332fa" />
<img width="690" height="856" alt="image" src="https://github.com/user-attachments/assets/2c2c09ba-4f61-4140-9f5a-af2e17e904da" />
Soal (Permintaan),Jawaban (Perintah yang Benar)
pindah ke direktori home kamu!,cd atau cd ~
tampilkan path direktori sekarang!,pwd
buat satu direktori bernama temp!,mkdir temp
pindah ke direktori temp!,cd temp
salin file /etc/shells ke direktori ini!,cp /etc/shells .
ubah nama file shells menjadi sh!,mv shells sh
"tampilkan kalender, lalu redirect keluarannya ke file cal.txt!",cal > cal.txt
ubah permission file cal.txt agar bisa ditulis oleh orang lain (other)!,chmod o+w cal.txt
buat symlink direktori /usr/local ke direktori ini!,ln -s /usr/local .
tampilkan list isi direktori ini dengan format panjang!,ls -l
pindah ke direktori parent!,cd ..
hapus direktori temp seisinya!,rm -r temp
#2
Soal (Permintaan),Jawaban (Perintah yang Benar)
gunakan locate untuk mencari file bernama stdlib.h!,locate stdlib.h
gunakan find untuk mencari file di /usr/include yang namanya diawali g!,find /usr/include -name 'g*'
gunakan wc untuk menghitung jumlah baris pada file /usr/include/stdlib.h!,wc -l /usr/include/stdlib.h
"tampilkan isi file /etc/passwd, lalu pipe untuk ambil kolom ke-7 (delimiter ':'), urutkan, dan hilangkan duplikat!",cat /etc/passwd | cut -d: -f7 | sort | uniq
#3
Soal (Permintaan),Jawaban (Perintah yang Benar)
tampilkan nama komputer!,hostname
tampilkan alamat IP komputer!,ip addr atau ip a
tampilkan nama kernel!,uname atau uname -s
tampilkan tanggal dan waktu sistem!,date
tampilkan daftar user yang sedang login!,who
jalankan sleep 500 pada background dengan nilai awal nice 15!,nice -n 15 sleep 500 &
tampilkan daftar proses dengan format panjang (-l)!,ps -l
kirim sinyal STOP ke proses tersebut! (gunakan nomor job),kill -STOP %<nomor_job>
tampilkan daftar job!,jobs
kirim sinyal CONT ke proses tersebut! (gunakan nomor job),kill -CONT %<nomor_job>
lanjutkan proses tersebut pada foreground! (gunakan nomor job),fg %<nomor_job>
