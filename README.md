# latihan-revert

Ini latihan buat revert di Git. Setiap ada perubahan di file ini bakal nambah 1 baris dan nambah 1 commit.

1. Saya habis nulis di readme.
2. Saya tambahin baris baru di readme.
3. Saya bikin branch `uat` dari branch `master`, lalu saya push ke branch `uat`, dan saya pull request ke branch `master`.
4. Saya bikin branch `development` dari branch `uat`, lalu saya push ke branch `development`, terus pull request dari branch `development` ke branch `uat`, dan terakhir pull request dari branch `uat` ke branch `master`.
5. Saya bikin alur kayak gini: setiap perubahan di push ke `development`, lalu dari `development` pull request ke `uat`, dan dari `uat` pull request ke `master`.
6. Tapi, saya bikin kesalahan. Saya udah ubah sesuatu di branch `development` tapi saya langsung PR ke `master` tanpa lewat `uat`. Jadinya, habis itu saya PR juga dari `development` ke `uat`. 
7. Sejak saat itu, setiap saya merubah file di `development`, saya PR dari `development` ke `uat`, lalu PR lagi dari `development` ke `master`.
8. Jujur, pengennya alur PR balik lagi kayak normal. Coba di cek perbedaan filenya dari `uat` ke `master`. Kalo ada yang aneh dan kalo bisa, dari `master` coba revert ke commit yang isinya baris terakhir itu baris ke-5.
9. Tes ya, ternyata masih belum bisa ges...
10. Tes sekali lagi ya, kalo bisa PR pake alur normal, berarti berhasil.