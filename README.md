# rAthenaID - Proyek Penerjehaman Bahasa Indonesia

Daftar isi
---------
1. Tentang proyek
2. Cara menggunakan
3. Mengubah bahasa default
4. Cara berkontrobusi
5. Credits

## 1. Tentang proyek
Proyek ini adalah proyek terpisah dari [rAthena](https://github.com/rathena/rathena) yang menyediakan file-file terjemahan ke dalam Bahasa Indonesia.

## 2. Cara menggunakan
  1. Buka file [languages.conf](https://github.com/rathena/rathena/blob/master/conf/languages.conf) pada emulator rAthena.
  2. Tambahan data baru pada daftar `languages` dengan cara copy semua isi file `file_list.conf`.
  3. Copy semua folder dan file dari `lang/Indonesian` ke [lang/Indonesian](https://github.com/rathena/rathena/blob/master/lang/) pada folder rAthena

Contoh hasilnya seperti berikut:

```
// ...
// List of languages.
languages: {
	// ...
	Bahasa_lain: {
		lang: (
			"lang/bahasa_lain.po"
		)
	}
	// ...

	Indonesian: {
		// File terjemahan dari conf/motd.txt
		motd: "lang/Indonesian/motd.txt"
		// File terjemahan dari conf/help.txt
		help: "lang/Indonesian/help.txt"
		// File terjemahan untuk masing-masing file NPC,
		// dapat diklasifikasi sesuai dengan struktur folder dan file asli dari rAthena
		// Berikut adalah terjehaman yang tersedia saat ini:
		lang: (
			"lang/Indonesian/msg_conf.po",
			"lang/Indonesian/npc/airports/airship.po",
			"lang/Indonesian/npc/kafras/kafras.po",
			"lang/Indonesian/npc/re/cities/malangdo.po",
			"lang/Indonesian/npc/re/jobs/novice/novice.po"
		)
	}

	// ...
}
```

## 3. Mengubah bahasa default

### Untuk pemain
  1. Pastikan pemain dapat menggunakan perintah `@langtype`.
  2. Gunakan perintah `@langtype Indonesian`.

### Untuk server
Jika ingin menjadikan **Bahasa Indonesia** menjadi bahasa default pada server, maka ikuti langkah berikut:
  1. Buka file [languages.conf](https://github.com/rathena/rathena/blob/master/conf/languages.conf) pada emulator rAthena.
  2. Pastikan terjemahan Bahasa Indonesia sudah ditambahkan.
  3. Ubah pada `default_language: "English"` menjadi `default_language: "Indonesian"`.

## 4. Cara berkontrobusi
Siapa saja diperkenankan untuk berkontribusi baik untuk menambahkan terjemahan ataupun memperbaiki.

### Pull Request
  1. Pastikan sudah memiliki akun [Github](https://github.com).
  2. Lakukan [fork](https://help.github.com/articles/fork-a-repo/) repository ini.
  3. Sebelum melakukan perubahan, pastikan sudah [membuat branch baru](https://help.github.com/articles/creating-and-deleting-branches-within-your-repository/) sebagai tempat untuk melakukan perubahan.
  4. Setelah selesai melakukan perubahan, pastikan lakukan commit dan push ke repository.
  5. Buatlah [Pull Request](https://help.github.com/articles/creating-a-pull-request/) untuk rAthenaID.

Perlu diingat, apabila menerjemahkan ke Bahasa Indonesia, **DILARANG KERAS** menggunakan tool penerjemah tanpa melakukan pengecekan ulang.

### Laporkan kesalahan
Apabila terjadi kesalahan dalam penerjemahan, harap laporkan dengan menuliskannya pada [Issue](https://github.com/pservero/rAthenaID/issues/new) di repository ini.

## 5. Credits
@Cydh @nanakiwurtz
