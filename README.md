# UAP-ML

## Deskripsi Dataset
Dataset Kaggle: https://www.kaggle.com/datasets/rashmiranu/banking-dataset-classification/data
Dataset ini berkaitan dengan kampanye pemasaran langsung dari sebuah institusi perbankan di Portugal. Kampanye pemasaran dilakukan melalui panggilan telepon, dan sering kali memerlukan lebih dari satu kontak dengan klien untuk mengetahui apakah mereka akan berlangganan deposito berjangka bank ("ya") atau tidak ("tidak").

Bank ini sedang menghadapi penurunan pendapatan karena banyak nasabah yang tidak cukup berinvestasi dalam deposito berjangka. Oleh karena itu, tujuan dari analisis ini adalah untuk mengidentifikasi nasabah yang memiliki kemungkinan lebih tinggi untuk berlangganan deposito berjangka dan memfokuskan upaya pemasaran pada segmen tersebut.

## Informasi Dataset
Dataset terdiri dari dua file utama:

1. **train.csv**:
   - Berisi 32.950 data dengan 21 fitur (termasuk fitur target "y").
   - Data ini diurutkan berdasarkan tanggal (Mei 2008 hingga November 2010).

2. **test.csv**:
   - Berisi 8.238 data dengan 20 fitur (tanpa fitur target "y").
   - Data ini sudah melalui tahap praproses.

### Tujuan
Tujuan dari klasifikasi ini adalah untuk memprediksi apakah seorang klien akan berlangganan deposito berjangka (variabel "y").

### Fitur pada Dataset
Berikut adalah daftar fitur yang terdapat pada dataset:

#### Fitur pada Data Latih dan Uji
| Feature       | Feature Type              | Description                                                                                       |
|---------------|---------------------------|---------------------------------------------------------------------------------------------------|
| age           | numeric                   | Age of a person                                                                                  |
| job           | categorical, nominal      | Type of job ('admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown') |
| marital       | categorical, nominal      | Marital status ('divorced','married','single','unknown'; note: 'divorced' means divorced or widowed) |
| education     | categorical, nominal      | Level of education ('basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown') |
| default       | categorical, nominal      | Has credit in default? ('no','yes','unknown')                                                   |
| housing       | categorical, nominal      | Has housing loan? ('no','yes','unknown')                                                        |
| loan          | categorical, nominal      | Has personal loan? ('no','yes','unknown')                                                       |
| contact       | categorical, nominal      | Contact communication type ('cellular','telephone')                                              |
| month         | categorical, ordinal      | Last contact month of year ('jan', 'feb', 'mar', …, 'nov', 'dec')                                |
| day_of_week   | categorical, ordinal      | Last contact day of the week ('mon','tue','wed','thu','fri')                                     |
| duration      | numeric                   | Last contact duration, in seconds. Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no') |
| campaign      | numeric                   | Number of contacts performed during this campaign and for this client (includes last contact)    |
| pdays         | numeric                   | Number of days that passed by after the client was last contacted from a previous campaign (999 means client was not previously contacted) |
| previous      | numeric                   | Number of contacts performed before this campaign and for this client                           |
| poutcome      | categorical, nominal      | Outcome of the previous marketing campaign ('failure','nonexistent','success')                  |

#### Variabel Target
| Feature       | Feature Type  | Description                                                                                       |
|---------------|---------------|---------------------------------------------------------------------------------------------------|
| y             | binary        | Has the client subscribed a term deposit? ('yes','no')                                            |
