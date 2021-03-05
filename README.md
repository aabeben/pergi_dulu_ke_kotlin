# pergi_dulu_ke_kotlin

## Menggunakan keyword `if`

Sebuah percobaan `if` adalah serupa pada percobaan di dalam sebuah `while` hanya saja sebagai ganti dari perkataan "
selagi masih ada es krim..." Anda katakan "Jika masih ada es krim..."

Agar supaya anda dapat melihat bagaimana ia bekerja, inilah beberapa kode yang mencetak sebuah untaian jika sebuah angka
lebih besar daripada angka yang lainnya:

```kotlin
    fun main(args: Array<String>) {
        val x = 3
        val y = 1
        if (x > y) {
            println("x lebih besar daripada y")
        }
        println("Baris ini akan berlari biar bagaimanapun")
    }
```

Kode di atas mengeksekusi si baris yang mencetak "x ialah lebih besar daripada y" hanya jika si kondisi (x lebih besar
daripada y) bernilai benar. Tidak memandang apakah bernilai benar, sekalipun, si baris yang mencetak "Baris ini akan
berlari biar bagaimanapun" akan berlari. Jadi bergantung pada nilai-nilai dari x dan y, baik satu pernyataan atau dua
akan dicetak.

Kita dapat juga menambahkan sebuah `else` pada si kondisi, sehingga kita dapat berkata sesuatu seperti berikut, "Jika
masih terdapat es krim, terus sendoki, jika tidak maka makanlah si es krim kemudian beli lagi".

Berikut adalah versi terbaru dari kode di atas yang terdapat sebuah `else:`

```kotlin
    fun main(args: Array<String>) {
        val x = 3
        val y = 1
        if (x > y) {
            println("x lebih besar daripada y")
        } else {
            println("x tidak lebih besar daripada y")
        }
        println("Baris ini akan berlari biar bagaimanapun")
    }
```

Pada kebanyakan bahasa-bahasa, pembahasan tentang `if` selesai sampai di sini; Anda menggunakannya untuk mengeksekusi
kode jika kondisi-kondisi terpenuhi. Namun Kotlin masih ada kelanjutannya.

Pada Kotlin, Anda bisa menggunakan `if` sebagai sebuah ekspresi, sehingga ia mengembalikan sebuah nilai. Semisal "Jika
masih ada es krim di dalam baki, kembalikan satu nilai, jika tidak kembalikan nilai yang lainnya". Anda dapat
menggunakan bentuk `if` ini untuk menuliskan kode yang lebih ringkas.

Marilah kita lihat bagaimana ia bekerja dengan mengerjakan ulang si kode yang telah Anda lihat pada halaman sebelumnya.
Sebelumnya, kita telah gunakan kode berikut untuk mencetak sebuah untaian:

```kotlin
    if (x > y) {
        println("x lebih besar daripada y")
    } else {
        println("x tidak lebih besar daripada y")
    }
```

Kita dapat menulis ulang dengan cara menggunakan ekspresi `if` seperti berikut:

```kotlin
    println(if (x > Y) "x lebih besar daripada y" else "x tidak lebih besar daripada y")
```

Si kode:

```kotlin
    if (x > y) "x lebih besar daripada y" else "x tidak lebih besar daripada y"
```

adalah si ekpresi if. Ia memeriksa si kondisinya if pertama kali: `x > y`. Jika kondisi ini bernilai benar, si ekspresi
mengembalikan si untaian "x lebih besar daripada y". Selainnya (`else`) si kondisi bernilai salah, dan si ekspresi
mengembalikan si untaian "x tidak lebih besar daripada y" sebagai gantinya.

Si kode kemudian mencetak si nilainya ekspresi `if` menggunakan `println`:

```kotlin
    println(if (x > y) "x lebih besar daripada y" else "x tidak lebih besar daripada y")
```

Jadi jika `x` lebih besar daripada `y`. "x lebih besar daripada y" dicetak. Jika tidak, "x tidak lebih besar daripada y"
lah yang dicetak.

Sebagaimana telah anda lihat sendiri, menggunakan sebuah ekspresi `if` memiliki efek yang sama seperti si kode yang
telah anda lihat pada halaman sebelumnya, tapi lebih ringkas.


Marilah kita ujicoba nyetir.

Larikanlah si kode dengan pergi ke menu **Run**, dan memilih si perintah **Run 'AppKt'. Si teks berikut mestinya tampil pada si jendela keluaran di bagain bawahnya si IDE:

x lebih besar daripada y

Baris ini akan berlari biar bagaimanapun

Sekarang Anda telah pelajari bagaimana menggunakan `if` untuk percabangan terkondisi dan ekspresi-ekspresi, Lanjutkan ke latihan berikut.

```kotlin
   fun main(args: ArrayList<String>){
       var x = 1
    
        while (x < ...){
            ... ( if (x == ...) "Yab" else "Dab")
            ... ("ba")
            x = x + 1
        }
        if ( x == ... ) println("Do")
   } 
```

* `println`
* `print`
* 4
* 3
* 2
* 2
* 3
* 1
* `print`
* 4
* 1
* `println`

## Menggunakan si cangkang interaktifnya Kotlin

Kita sedikit lagi sampai di akhir bab, tetapi sebelum kita pergi, Masih ada satu lagi yang kita inginkan untuk diperkenalkan kepada Anda: si cangkang interaktifnya Kotlin, atau **REPL**. si REPL mengizinkan anda untuk mencoba potongan-potongan kode di luar kode `main` secara cepat.

> CATATAN
>  REPL singakatan dari **R**ead-**E**val-**P**rint-**L**oop, namun tidak ada seorangpun yang menyebut demikian.
> 

Anda buka si REPL dengan pergi ke menu **Tools** di dalam IntelliJ IDEA dan memilih Kotlin --> Kotlin REPL. Dengan demikian sebuah panel baru akan terbuka pada bagian bawah dari layar seperti berikut:
