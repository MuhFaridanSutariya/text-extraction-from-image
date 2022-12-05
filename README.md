# Aplikasi pembaca teks pada gambar

![image](https://user-images.githubusercontent.com/88027268/205564653-589e8e1e-52b2-4a64-b630-35a5686a2abe.png)

Gambar 1. Tampilan awal aplikasi

## Proyek overview

Sebuah proyek yang dibuat untuk dapat memudahkan manusia dalam pengambilan teks dari sebuah gambar secara cepat dan tepat dengan mengimplementasikan teknik *Optical Character Recognition* atau ekstraksi teks dari sebuah gambar. proyek ini masih dapat dikembangkan dengan menggunakan teknologi canggih seperti salah satunya adalah *BERT*. Aplikasi ini telah dilakukan deployment ke sebuah website menggunakan teknologi *flask*.

## Teknologi yang digunakan

- opencv
- pytesseract
- tesseract
- numpy
- Flask
- Pillow


## Langkah-langkah untuk menjalankan aplikasi ini:
-	Clone repository ini atau melakukan download manual.
- Buka command prompt atau miniconda lalu masuk ke path yang dimana pada path tersebut dapat mencari file *app.py* secara langsung.
- Buat environment pada path tersebut - conda create -name <environment name>
- Activate environment pada path tersebut sesuai dengan environment yang telah dibuat sebelumnya - conda activate <environment name>
- Install tesseract sesuai dengan operasi sistem yang dimiliki - https://github.com/UB-Mannheim/tesseract/wiki
- Dapat memindahkan hasil installan ke path yang sesuai. Default path setelah didownload: C:\ProgramFiles\Tesseract-OCR
- Setelah itu dapat menambahkan environment variable sesuai dengan path installer. Seperti gambar dibawah:

![image](https://user-images.githubusercontent.com/88027268/205570664-84705e5b-2e89-43ae-be63-d575abc56fd6.png)

Gambar 2. Tampilan menambahkan environment variable

- pytesseract.pytesseract.tesseract_cmd = r'C:\ProgramFiles\Tesseract-OCR\tesseract.exe' Ganti sesuai dengan path yang telah diinstall sebelumnya pada file *views.py* dari folder *app*.
- Gunakan command berikut untuk melakukan install dependencies yang dibutuhkan - python -m pip install -r requirements.txt
- Jalankan aplikasi yang telah dibuat dengan command berikut - python app.py
Setelah berjalan dengan baik maka dapat copas link tersebut ke browser. contoh: http://127.0.0.1:5000/ 
- Telah disediakan sample gambar yang dapat dilakukan ujicoba pada aplikasi tersebut.

## Kesimpulan:
Dimulai dengan mempelajari cara menginstall tesseract yang digunakan untuk ekstraksi teks. Selanjutnya mengambil gambar dan mengekstrak teks dari gambar itu. Mendapatkan pelajaran yang penting yaitu bahwa perlu menggunakan fungsi transformasi gambar tertentu dari OpenCV untuk mengekstraksi teks dari gambar yang kompleks.
  
## Reference:
- [(Blog medium yang ditulis oleh Simón Cerda, 2021)](https://medium.com/@simsagues/document-information-extraction-using-ocr-and-nlp-2c3caa5a7720)
- [(Margot Mieskes dan Stefan Schmunk, 2019)](https://paperswithcode.com/paper/ocr-quality-and-nlp-preprocessing)
