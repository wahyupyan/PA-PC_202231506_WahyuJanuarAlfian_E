# PA-PC_202231506_WahyuJanuarAlfian_E
Penjelasan Project Akhir (UAS) Pengolahan Citra Digital
# 1. Fungsi untuk Menampilkan Gambar
## Penjelasan Dari Menampilkan gambar:
    def show_images(images, titles):
        plt.figure(figsize=(20, 20))
        for i in range(len(images)):
            plt.subplot(2, 3, i+1)
            plt.imshow(cv2.cvtColor(images[i], cv2.COLOR_BGR2RGB))
            plt.title(titles[i])
            plt.axis('off')
        plt.show()
- Parameter:
1. images : Daftar gambar yang akan ditampilkan.
2. titles : Daftar judul untuk setiap gambar.

- Tujuan: Fungsi ini bertujuan untuk menampilkan beberapa gambar dalam satu figure menggunakan Matplotlib.
- Proses:
1. Mengatur ukuran figure menjadi 20x20.
2. Menggunakan subplot untuk mengatur tata letak gambar dalam grid 2x3.
3. Mengubah format gambar dari BGR (format default OpenCV) ke RGB agar warna ditampilkan dengan benar.
4. Menampilkan setiap gambar dengan judul masing-masing dan tanpa sumbu.




