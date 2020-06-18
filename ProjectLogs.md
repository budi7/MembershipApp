#Meeting 1
##18 Juni 2020

### policy detail
-> member number : mau dipake seperti apa? format numbering sperti apa?
-> apa running expired? jadi problem tdk, serving bisnis yg membernya expired atau tdk? prblemnya, untuk setup bisnis owner lumayan ribet, apa fitur ini jadi poin plus atau poin minus
-> special promo: manual, karena blm ada POS. 
-> poin, buka fitur nya bgmn, generic (bisnis owner bisa tambah poin terserah dia) atau rupiah, lalu poin ini di pakai buat apa?

-----

1. QR Code:
-> generate dari member nember
-> security issue: qr code baru kepake waktu penjual dan pembeli ketemu, qr code dipakai validasi bahwa org yg pake voucher adalah org yg punya. 
    -> qr code sebaiknya di generate dengan security code 
    
    * notes: [apps] waktu display code, harus terlebih dulu fetch code sblm tampilkan qr 
    * target: bisa di pakai cust aqusition, & cust retention

2. Member number
-> auto generate, per member per bisnis

3. Member expires
-> menerapkan atau tidak? member expired nya ke aplikasi, bukan ke bisnis

4. Member Point
-> Per tenant, point hanya bisa dipakai dan didapatkan di tenant yg sama. 
-> Penambahan point, lgsg point kemudian (next dev) di konversi ke IDR.
-> Untuk point, di level tenant. Point di tenant A dan tenant B tdk tersambung. 

5. Member voucher
-> tenant dikasih pilihan voucher apa, dikeluarkan berapa.
-> voucher hanya caption saja, terserah tenant bisa create isi voucher, jumlah brp, expired kapan.
-> input: 
    - judul
    - syarat: diketik manual (text freeflow) krn tdk handle transaksi  
    - nominal diskon potongan berapa

6. Outlet List
-> basic info, sperti comp. profile

7. Special Promo
-> Halaman list daftar promonya apa aja (utk semua tenant)
-> kalo bayar, nanti urutan bisa di atur

-----

1. member profile 
-> data yg didaftarkan 
    - no telpon
    - email (optional)
    - tgl lahir (optional)
    - jenis kelamin 
-> edit profile 

2. edit profil
standard  

-----

1. voucher list
standard semua 

-----

1. notifilasi pake FCM, tidak pake sms

-----

1. Inbox msg
-> kirim info dari tenant ke user

2. Tag member : multiple tagging

-----

1. export member -> csv (sementara hide dulu)

-----

1. event page 
-> halaman company profile, banner feed

-----

1. Point
pensius -> makan berapa jadi poin, di halaman apps bisa beli voucher. 
poin -> ditukar voucher. User sendiri yg kumpulin sendiri, konversi sendiri.

menyiapkan voucher mana yg bisa di beli end user, dan mana yg ga bisa dibeli (hanya bisa di berikan oleh tenant)

expiry poin -> tanpa expiry point untuk semntara 

2. send email on birthday
-> email yg di kirim di compile jadi satu

3. send voucher
standrad 

-----

1. Pricing
-> entry level (100 member) : free 
-> next level, di matangkan lagi
-> untuk iklan banner, dijual diluar membership

------
## Technical 
- server : dari thunderlab
- ios account: dari thunderlab 

## Timeline :
1. API -> 1 minggu
2. paralel: dessain jalan, dari API desain basic fitur

## next meeting: 
25 jun 2020, 15:00
