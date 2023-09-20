# Variables

Sering kali, aplikasi JavaScript perlu bekerja dengan informasi. Berikut adalah dua contohnya

1. Sebuah toko online - informasi mungkin termasuk barang yang dijual dan keranjang belanja.
2. Aplikasi chatting - informasi mungkin termasuk pengguna, pesan, dan banyak lagi

Variabel digunakan untuk menyimpan informasi ini

## A variable

Sebuah variable bisa juga disebut "penyimpanan bernama" untuk data. Di Javascript kita menggunakan sintaks `let` dan `const` untuk membuat sebuah variabel. Perbedaannya adalah:

1. `let`: nilai yang ada di variabel ini dapat berubah
2. `const`: nilai yang ada di variabel tersebut tidak dapat diubah

Di bawah ini kita mendeklarasi sebuah variabel dengan menggunakan `let`

```javascript
let message; //deklarasi

message = "Halo Bwang"; //inisialisasi
```

Yang kulakukan diatas adalah **deklarasi** dan **inisialisasi**

1. Deklarasi adalah proses mengalokasikan sebuah memori untuk menyimpan sebuah data, simpelnya untuk memberikan kita ruang untuk meletakkan nilai
2. sementara inisialisasi adalah sebuah proses untuk memberikan sebuah nilai

Kita dapat menyingkat kedua proses tersebut menjadi satu seperti ini:

```javascript
let message = "Halo Bwang";
```

Kita juga dapat mendeklarasikan banyak variabel seperti ini:

```javascript
let user = "Fahri",
	age = "19",
	message = "Mantap puh";
```

## A real-life analogy

Kita dapat membayangkan variabel itu seperti sebuah kotak yang berisi data, dengan label nama di depan box tersebut<br>
Sebagai contoh, ada variabel message yang bisa kita bayangkan seperti sebuah kotak dengan label "message" dan bernilai "Hello!" <br>
![box](img/box.png)<br>
Kita juga dapat mengubah nilai yang ada di dalam box

```javascript
let message;

message = "Hello!";

message = "World!"; // value changed
```

Ketika kita mengubah nilainya, maka nilai yang lama akan hilang

![ubah-nilai-box](img/ubah-nilai-box.png)

Kita juga dapat mengcopy variabel satu ke yang lain

```javascript
let hello = "Hello world!";

let message;

// copy 'Hello world' from hello into message
message = hello;
```

> ### (WARNING)Mendeklarasi dua kali akan menyebabkan error
>
> variabel hanya dapat dideklarasi satu kali
>
> ```javascript
> let message = "This";
>
> // repeated 'let' leads to an error
> let message = "That"; // SyntaxError: 'message' has already been declared
> ```
>
> <br>
