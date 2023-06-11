# Klasifikasi Jenis Bunga Menggunakan Metode Depp Learning Convolutional Neural Network(CNN)
Tentang Klasifikasi Jenis Bunga Menggunakan Metode Depp Learning Convolutional Neural Network(CNN)<br><br>
<b>Penyusun :</b>
1. Subairi (21081010019) <br>
2. Muhammad Abdullah Hafizh (21081010099)<br>
3. Raditya Dimas Libriawan (21081010157) <br>
 
<b> Kelas : Kecerdasan Buatan E081</b><br>
  
# Ilustrasi Metode Covolutional Neural Network
<p align="center">
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/CNN.png" alt="" class="img-responsive" width="700">
</p> <br>

# File dan program yang dibutuhkan
1. Data set dari https://gitlab.com/ykristian/dataset-bunga <br>
2. Module Program Python antara lain: <br>
    - numpy <br>
    - pickle <br>
    - glob <br>
    - matplotlib <br>
    - cv2 <br>
    - pandas <br>
    - sklearn <br>
    - Keras <br>
    - PIL(pillow) v
    - .
4. Script Program untuk run program menggunakan Python Jupyter Notebook (klasifikasi bunya.ipynb)[https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/Klasifikasi%20bunga%20CNN.ipynb].<br><br>

# Langkah-langkah dalam program

1. import library python yang dibutuhkan <br>
   <p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 1.png" alt="" class="img-responsive" width="600">
</p><br>
2.  import dataset bunga (dapat menggunakan gitclone atau langsung diletakkan ke dalam folder kerja jupyter notebook) <br>
   <p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 2.png" alt="" class="img-responsive" width="600">
</p><br>
3.  Identifikasi data, cek dan test label data dan image data <br>
   <p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 3.png" alt="" class="img-responsive" width="600">
</p><br>
4.  Identifikasi data dan neuron pada data serta posisi indeks True(1)/false(0) yg digunakan untuk melabeli semua data  <br>
    sesuai dengan label 0=Daisy 1=Dandelion 2=Rose 3=Sunflower 4=Tulip <br>
   <p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 4.png" alt="" class="img-responsive" width="700">
</p><br>
5. Membagi Training dan Testing set, dengan size Training set =0.8 dan Testing set =0.2 <br>
   <p>
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 5.png" alt="" class="img-responsive" width="700">
</p><br>
6. Mengimport model pretrained network yang akan digunakan dari keras aplication, kami memilih model EfficientNetV2M<br>
   <p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 6.png" alt="" class="img-responsive" width="700">
</p><br>
7. Menambahkan layer model yg dibutuhkan  <br>
   <p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 7.png" alt="" class="img-responsive" width="700">
</p><br>
8. Melakukan proses freezing dengan cara mengurangi trainable layer pada model dengan tujuan untuk mempercepat proses training data  <br>
   <p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 8.png" alt="" class="img-responsive" width="700">
</p>
Proses diatas dapat mengurangi weight parameter dari 65 juta menjadi 15 juta sehingga proses training akan lebih cepat. <br><br>
9. Melakukan Proses training menggunakan modul Adam yang disediakan keras aplication dengan epoch sebanyak 10 kali  <br>
   <p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 9.png" alt="" class="img-responsive" width="700">
</p>
Dari training sebanyak 10 epoch sudah dihasilkan rata-rata akurasi yg tinggi, sehingga model siap dan layak untuk digunakan. <br><br>
10. Testing dilakukan dengan menggunakan gambar dari internet untuk diidentifikasi <br>
   <p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 10.png" alt="" class="img-responsive" width="700">
</p>
<p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 10.1.png" alt="" class="img-responsive" width="700">
</p><br>
11. Melemparkan gambar yg dimasukkan pada model untuk diidentifikasi<br>
   <p >
  <img src="https://github.com/subaaaiii/CNN-Klasifikasi-Bunga/blob/main/step 11.png" alt="" class="img-responsive" width="600">
</p>
Akan ditampilkan hasil dari proses identifikasi sudah sesuai dengan indeks yang ada.


