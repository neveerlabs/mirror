<a align="center">
    <h1>Mirror</h1>
    <p><i>Alat untuk membandingkan sebuah project dari <b>lokal</b> dengan repo <b>Github</b></i></p>
</a>

## Struktur file
```
mirror/
├── view.py     # script utama
└── .viewrc     # file data
```

## Tutorial implementasi
1. Clone repositori
    ```bash
    git clone https://github.com/neveerlabs/mirror.git && cd mirror
    ```
2. Copy file dan pindahkan pada folder project
    ```bash
    cp view.py /home/user/project/
    ```
3. Run program
    ```bash
    python3 view.py
    ```
    Saat script running, script akan meminta data **owner repo**, lalu menyimpan datanya di file `.viewrc` di path project tersebut.

## Yang dilakukan oleh script
- membaca seluruh isi file & folder raw repo lalu membandingkannya dengan data project lokal.
- data `owner`, `brand` dan `repo` disimpan didalam file `.viewrc`

## Pemberitahuan
- **`[0]`** artinya sama dan **`[1]`** berbeda
- tidak perlu menggunakan `token classic`
- script ini bertujuan untuk membaca dan membandingkan file dan folder dari lokal dengan yg di repo supaya mudah untuk backup
- satu **script** mirror ini hanya untuk satu **project**!
- file `view.py` harus disimpan didalam folder setiap **project!** Bukan di folder repo ini (`mirror`)!

---

<a align="center">
    <p><b>Made with by Neverlabs</b></p>
</a>
