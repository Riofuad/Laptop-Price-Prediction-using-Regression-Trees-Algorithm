# Laptop-Price-Prediction-using-Regression-Trees-Algorithm
**TEAM NIHONGO**
**Members:**
- H071201033 | Muhammad Haerul
- H071201041 | Muhammad Azhar Tawakkal
- H071201045 | Faizah Mappanyompa
- H071201050 | Iman Mustika Ismail

## Dataset Knowledge
<p align="justify">
Dataset yang akan digunakan dalam pembuatan model adalah dataset ‘Laptop Price’ yang disusun oleh seorang freelance asal Turki yang bergerak di bidang Data Science yang bernama Muhammet Varlı. Dataset tersebut memiliki skor usability sebesar 10.0 yang artinya dataset tersebut memiliki informasi yang sangat lengkap. Selain itu, dataset ini juga telah di-upvote oleh 99 orang dan telah memperoleh bronze medal dalam hal popularitas dataset. Dataset ini dapat diperoleh dari link https://www.kaggle.com/datasets/muhammetvarl/laptop-price. Dataset ini berisikan mengenai data spesifikasi laptop beserta harganya. 
	
	Dataset ini terdiri atas beberapa atribut:
	1. Company. Atribut ini berisikan mengenai nama merek atau perusahaan yang menghasilkan laptop tersebut. Atribut ini berisikan data yang bertipe String atau dalam IPYNB bertipe Object. Contoh data atribut ini seperti Apple, Asus, Lenovo, dsb. 
	2. Product. Atribut ini berisikan model atau nama dari suatu laptop. Atribut ini berisikan data yang bertipe String atau dalam IPYNB bertipe object. Contoh data atribut ini seperti Macbook Pro, Legion Y520-15IKBN, Aspire 3, dsb.
	3. TypeName. Atribut ini berisikan tipe dari suatu laptop. Atribut ini berisikan data yang bertipe String atau dalam IPYNB bertipe Object. Atribut ini hanya terdiri atas 6 nilai, yaitu Notebook, Gaming, Ultrabook, 2 in 1 convertible, Workstation, dan Netbook.
	4. Inches. Atribut ini berisikan ukuran layar laptop dalam satuan inci. Atribut ini berisikan data yang bertipe numerik atau dalam IPYNB bertipe float64. Atribut ini memuat data ukuran laptop mulai dari yang terkecil 10,1 inci hingga yang terbesar 18,4 inci.
	5. ScreenResolution. Atribut ini berisikan ukuran resolusi laptop atau seberapa banyak piksel yang dapat ditampilkan oleh layar laptop serta tipe layar yang digunakan pada laptop. Semakin tinggi resolusinya maka semakin banyak pula pixel yang dapat ditampilkan dan layar semakin tajam. Atribut ini berisikan data yang bertipe String atau dalam IPYNB bertipe object. Beberapa contoh data untuk atribut ini antara lain Full HD 1920x1080 dan IPS Panel Full HD 1920x1080.
	6. CPU. Atribut ini berisikan jenis CPU yang digunakan dalam laptop. Atribut ini berisikan data yang bertipe String atau dalam IPYNB bertipe Object. Data dalam atribut ini menjelaskan merek CPU apa yang digunakan, seri ke berapa, dan kekuatan dari CPU yang digunakan. Beberapa contoh dari atribut ini antara lain Intel Core i5 7200U 2.5GHz dan AMD A9-Series 9420 3GHz.
	7. RAM. Atribut ini menunjukkan besar kapasitas RAM yang dimiliki oleh Laptop dalam satuan GB. Atribut ini juga berisikan data yang bertipe data String atau Object dalam IPYNB. Data pada atribut ini berisi data RAM dimulai dari 2 GB hingga terbesar 64 GB.
	8. Memory. Atribut ini berisikan data mengenai kapasitas penyimpanan yang dimiliki oleh laptop serta jenis memori yang dapat digunakan (SSD/HDD/Flash Storage). Atribut ini berisikan data bertipe String atau bertipe Object dalam IPYNB. Data dalam atribut ini bisa berisikan dua nilai karena bisa saja sebuah laptop menggunakan dua jenis memori yang berbeda. Beberapa contoh nilai dari atribut ini adalah 256GB SSD dan 128GB SSD +  1TB HDD.
	9. GPU. Atribut ini berisikan GPU (Graphics Processing Unit)  apa yang digunakan dalam laptop. Data ini berisikan merek dari GPU serta nama seri dari GPU tersebut. Atribut ini berisikan data yang bertipe String atau Object dalam IPYNB. Beberapa contoh data untuk atribut ini antara lain Nvidia GeForce GTX 1050 dan AMD Radeon R5 M430.
	10. OpSys. Atribut ini berisikan OS yang digunakan dalam suatu laptop. Atribut ini berisikan data yang bertipe String atau Object dalam IPYNB. Beberapa contoh data untuk atribut ini antara lain Windows 10 dan MacOS.
	11. Weight. Atribut ini berisikan bobot yang dimiliki oleh laptop dalam satuan kg. Atribut ini berisikan data yang bertipe String atau Object dalam IPYNB. Beberapa contoh dari data ini adalah 2.3kg dan 2.2kg.
	12. Price_euros. Atribut ini berisikan data mengenai harga laptop dalam mata uang Euro. Atribut ini berisikan data yang bertipe numerik atau dalam IPYNB berbentuk float64. Atribut ini berisikan nilai yang beragam, mulai dari 174 Euro hingga 6099 Euro.
		
Berdasarkan alasan-alasan sebelumnya dan seberapa relate mahasiswa dengan laptop, maka diputuskan dataset ini akan digunakan untuk pembuatan model machine learning. Dataset ini dirasa cukup baik mengingat atribut-atribut yang digunakan dalam dataset memiliki kemungkinan berkorelasi dengan harga laptop.
</p>

## Model Purpose
<p align="justify">
Berdasarkan dataset tersebut, dapat dilihat bahwa salah satu model machine learning yang dapat dibuat adalah model regresi. Hal ini disebabkan karena salah satu label yang dapat dijadikan sebagai label target merupakan label Price_euros dimana kolom tersebut berisikan data harga yang bernilai kontinu. Sehingga, dengan menggunakan dataset tersebut, maka diputuskan akan dibuat sebuah model regresi untuk memprediksi harga suatu laptop berdasarkan atribut-atribut lainnya.
	Untuk membuat model prediksinya, maka akan digunakan berbagai model untuk mengetahui model mana yang dapat memprediksi harga laptop paling baik. 
	
	Model yang digunakan:
	1. Linear Model
	2. Decision Tree
	3. Random Forest
	4. XGBoost

Setelah membuat model-model tersebut, setiap model nantinya akan diuji akurasinya. Model dengan akurasi terbaik akan dipilih sebagai model akhir yang digunakan untuk memprediksi harga laptop nantinya.
</p>

## Result
<p align="justify">
	
	Hasil testing: 
	1. Model Linear Ridge Regression menghasilkan masing-masing r2 score 0.671, MAE 52% dan MSE 55%. 
	2. Model Decision Tree menghasilkan r2 score 0.728, MAE 45% dan MSE 46%. 
	3. Model Random Forest menghasilkan masing-masing r2 score 0.718, MAE 43% dan MSE 47%. 
	4. Model XGBoost menghasilkan r2 score 0.803, MAE 38% dan MSE 33%. 
</p>

## Conclusion
<p align="justify">
Dataset yang digunakan adalah dataset 'Laptop Price' untuk memprediksi harga laptop berdasarkan fitur-fitur yang diberikan. Agar dapat diproses oleh model, dilakukan data cleaning terlebih dahulu. Adapun prosesnya meliputi data formatting pada atribut Weight, Ram, Memory, Screen Resolution, dan Price. Data yang sudah diformat dilakukan encoding, yaitu metode mengubah data kategorik menjadi data numerik. Kemudian dilakukan feature selection menggunakan SelectKBest untuk mengurutkan atribut atau feature apa yang memiliki korelasi yang tinggi dengan target Price_IDR. Tahap terakhir, yaitu pembuatan dan evaluasi model. Ada beberapa model yang digunakan pada dataset ini yaitu Linear Model, Decision Tree, Random Forest, dan XGBoost. Dari model tersebut XGBoost mendapatkan nilai tertinggi dengan nilai akurasi sebesar 80%.
</p>

## Recomendation
Untuk penelitian selanjutnya dapat dilakukan data cleaning yang lebih akurat, menggunakan algoritma yang lebih baik dengan akurasi yang lebih tinggi untuk meningkatkan kinerja model. 
</p>

