# Nama : Dedy Kristianto Lumbantobing (tim : FE-12)

# Penjelasan

## Jawaban Nomor 1
### Soal :
1. Kita sudah mengetahui bahwa banyaknya user maksimal adalah 100.
Buat sebuah program yang menampilkan teks ‘User ke - 1 … User ke - 100’ pada setiap baris di halaman HTML.
Lakukan FOR LOOP pada Javascript.

### Jawaban :
jawaban tertera pada file [Jawaban Nomor 1.html](https://github.com/Dedytobing/tugas-KakTata/blob/main/JawabanNomor1.html "Github Dedy")

**Penjelasan ada pada comment pada kode berikut : **

```js
<div>
  <h1>Daftar User</h1>
  </div>
  <script>
    for (let i = 1; i <= 100; i++) {
      console.log('User ke - ' + i);
      document.write('User ke - ' + i + '<br>');
  }
  </script>
```

## Jawaban Nomor 2
### Soal :
2. Lakukan pengulangan menggunakan FOR LOOP untuk melakukan penambahan nilai sebanyak 10 kali.

- Nilai awal = 0
- Pengulangan = 10 kali
- Nilai awal ditambah 2 setiap pengulangan
- Tampilan hasil penambahan pada setiap pengulangan


### Jawaban :
jawaban tertera pada file [Jawaban Nomor 2.html](https://github.com/Dedytobing/tugas-KakTata/blob/main/JawabanNomor2.html "Github Dedy")

**Penjelasan ada pada comment pada kode berikut : **

``` javascript
 <script>
    let nilai_awal = 0;

    for (let i = 0; i < 10; i++) {
    nilai_awal += 2;
    document.write(`Hasil penambahan pada pengulangan ke-${i+1} adalah ${nilai_awal}` + '<br>');
    }

  </script>
```


## Jawaban Nomor 3
### Soal :
3.  Lakukan pengulangan dengan FOR LOOP yang melakukan iterasi dari 0..20.
- Setiap iterasi/pengulangan lakukan pengecekan apakah nilai tersebut ganjil atau genap.
- Tampilkan keterangan ganjil dan genap pada sebuah nilai setiap pengulangan


### Jawaban :
jawaban tertera pada file [Jawaban Nomor 3.html](https://github.com/Dedytobing/tugas-KakTata/blob/main/JawabanNomor3.html "Github Dedy")

**Penjelasan ada pada comment pada kode berikut : **

``` javascript
 <script>
    for (let i = 0; i <= 20; i++) {
      if (i % 2 === 0) {
        document.write(`${i} adalah bilangan genap` + '<br>');
      } else {
        document.write(`${i} adalah bilangan ganjil`+ '<br>');
      }
    }
  </script>
```




## Jawaban Nomor 4
### Soal :
4. Tampilkan sebuah Konfirmasi Pop Up kepada user menggunakan confirm();
-Berikan teks ‘Apakah anda mau mengulang’ pada box confirm
-Jika user memilih ‘OK’ maka program akan terus menampilan pop up yang sama
-Jika user memilih ‘Cancel’ maka program akan menampilkan teks ‘Perulangan sudah dilakukan sebanyak …(jumlah klik OK yang dilakukan user)




### Jawaban :
jawaban tertera pada file [Jawaban Nomor 4.html](https://github.com/Dedytobing/tugas-KakTata/blob/main/JawabanNomor4.html "Github Dedy")

**Penjelasan ada pada comment pada kode berikut : **

``` javascript
 <script>
    let count = 0;

  function showConfirmation() {
  const result = confirm("Apakah anda mau mengulang?");
  if (result) {
    count++;
    showConfirmation();
  } else {
    alert("Perulangan sudah dilakukan sebanyak " + count + " kali.");
  }
}

showConfirmation();

  </script>
```


## Jawaban Nomor 5
### Soal :
5. Buat sebuah program kuis.
Tampilkan prompt() untuk meminta inputan dari user. Tampilan teks ‘Sebutkan kepanjangan dari nama IB (Impact Byte)?’
- Lakukan pengecekan apakah jawaban dari user sudah benar
- Jika benar, tampilkan alert ‘Selamat jawaban kamu benar’
- Jika salah, lakukan pengulangan untuk menampilkan prompt() yg sama hingga jawaban dari user benar





### Jawaban :
jawaban tertera pada file [Jawaban Nomor 5.html](https://github.com/Dedytobing/tugas-KakTata/blob/main/JawabanNomor5.html "Github Dedy")

**Penjelasan ada pada comment pada kode berikut : **

``` javascript
 <script>
    let answer = "";
  while (answer !== "Impact Byte") {
  answer = prompt("Sebutkan kepanjangan dari nama IB (Impact Byte)?");
  if (answer === "Impact Byte") {
    alert("Selamat jawaban kamu benar");
  } else {
    alert("Maaf, jawaban kamu salah. Silakan coba lagi.");
  }
}
</script>
```

