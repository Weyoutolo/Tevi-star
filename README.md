# Tevi-star
Website top up star tevi 
# Membaca kode dari index.html sebelumnya dan memastikan QRIS sudah tertata dengan benar
with open("index.html", "r", encoding="utf-8") as f:
    content = f.read()

# Cek apakah nama file gambar QRIS sudah sesuai (IMG-20260720-WA0057_3.jpg atau tetap IMG-20260720-WA0057.jpg)
# Kita pastikan atribut src pada qrisInfo menggunakan gambar yang diunggah baru atau yang ada di kode.
# Di kode sebelumnya sudah menggunakan src="IMG-20260720-WA0057.jpg". Mari kita update namanya agar sesuai dengan file yang baru jika diperlukan, 
# atau biarkan merujuk ke file gambar QRIS yang baru.

content = content.replace('src="IMG-20260720-WA0057.jpg"', 'src="IMG-20260720-WA0057_3.jpg"')

with open("index.html", "w", encoding="utf-8") as f:
    f.write(content)

print("Berhasil memperbarui referensi gambar QRIS.")
