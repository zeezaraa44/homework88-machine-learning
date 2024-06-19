## homework88-machine-learning

#### Step by Step
1. Buka Google Colab
2. Install pandas dengan `!pip install pandas`
3. Download data pada [https://www.econometrics.com/intro/SALES.txt](https://www.econometrics.com/intro/SALES.txt) dengan `!wget https://www.econometrics.com/intro/SALES.txt`
4. Ganti judul kolom pada data dengan data.columns = ['Sales', 'Advertising']
5. Tampilkan informasi statistika deskriptif dari data menggunakan `print(data.describe())`
6. Menentukan data *Sales* sebagai variabel independen (X) dan data *Advertising* sebagai variabel dependen(y) dengan
   - `X = data['Sales'].values`
   - `y = data['Advertising'].values`
7. Ubah bentuk data X dan Y menjadi data kolom dengan
   - `X = X.reshape(-1,1)`
   - `y = y.reshape(-1,1)`
8. Membagi data menjadi data training dan data testing menggunakan fungsi `train_test_split`
9. Melakukan analisis regresi linear sederhana terhadap data training menggunakan fungsi `LinearRegression()`, melatih data training menggunakan fungsi `lm.fit(X_train, y_train)` dan melakukan prediksi menggunakan data testing dengan fungsi `lm.predict(X_test)`
10. Mendapatkan nilai intersep dan koefisien menggunakan `lm.intercept` dan `lm.coef`
11. Melakukan prediksi terhadap keseluruhan data menggunakan `lm.predict(X)`
12. Memprediksi nilai advertising apabila sales bernilai 50, 100, dan 150 menggunakan
    - print(str(lm.predict([[50]])))
    - print(str(lm.predict([[100]])))
    - print(str(lm.predict([[150]])))
14. Mencari nilai RMSE untuk mengukur kesalahan model dengan fungsi `mean_squared_error`
15. Mencari nilai R2 Score untuk mengukur keragaman variabel *Advertising* yang dapat dijelaskan oleh variabel *Sales*
16. Interpretasi 
