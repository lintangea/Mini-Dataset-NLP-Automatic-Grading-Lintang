# Mini-Dataset-NLP-Automatic-Grading-Lintang
Tugas NLP Mini Dataset Automatic Grading-Lintang Eka Adiastuti (2446000027)

Deskripsi Dataset :
Dataset berisi judul-judul penelitian atau artikel yang berkaitan dengan penggunaan _ Natural Language Processing_, khususnya dalam konteks pendidikan dan penilaian otomatis. Dengan jumlah data awal sebanyak 298, data ini mencakup berbagai aspek dari penerapan AI dalam pendidikan, penilaian otomatis, dan umpan balik berbasis AI.

Jumlah Baris: 298
Jumlah Kolom: 1
Nama Kolom : primary_title: object (teks)

Hasil Pembersihan Data (Cleaning Dataset)
  Script yang saya unggah mencakup langkah-langkah untuk melakukan prapemrosesan data dan analisis teks menggunakan Python, termasuk Filtering Duplicate, Parsing, Filtering Keyword, Tokenisasi, Stopword Removal, Lemmatization, pembobotan menggunakan TF-IDF, Insight Data dan Named Entity Recognition (NER).
  Pertama, kita mengimpor library yang diperlukan seperti pandas, nltk, dan spacy. Kemudian, kita memuat dataset yang berisi teks yang akan dianalisis. Setelah itu, kita melakukan tokenisasi pada kolom judul dokumen menggunakan nltk.tokenize.word_tokenize, yang memecah teks menjadi kata-kata. Selanjutnya, kita menghapus stopwords menggunakan daftar stopwords dari NLTK, yang berfungsi untuk menghilangkan kata-kata umum yang tidak memberikan banyak informasi. 
    Proses berikutnya adalah lemmatization, di mana kita mengubah kata-kata ke bentuk dasarnya menggunakan WordNetLemmatizer dari NLTK. Setelah mendapatkan kata-kata yang telah diproses, kita menerapkan pembobotan TF-IDF menggunakan TfidfVectorizer dari scikit-learn, yang memberikan bobot pada setiap kata berdasarkan frekuensinya dalam dokumen. Selanjutnya, kita menghitung frekuensi kata untuk mendapatkan kata-kata yang paling sering muncul dalam dataset. Kemudian, kita menerapkan NER menggunakan model spaCy untuk mendeteksi entitas dalam teks, seperti nama orang, organisasi, dan lokasi. Hasil NER disimpan dalam DataFrame dengan kolom yang menunjukkan nomor dokumen, judul dokumen, dan label entitas yang terdeteksi. Terakhir, kita dapat menampilkan hasil analisis, termasuk frekuensi kata, bobot TF-IDF tertinggi, dan entitas yang terdeteksi, memberikan gambaran yang disajikan mengenai data yang dianalisis.
