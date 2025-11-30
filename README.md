Rangkuman Praktikum Basis Data — BAB 3, 4, dan 5

Database: Order Entry System


---

📍 BAB 3 — Data Definition Language (DDL) Dasar

Topik Utama:

1. CREATE DATABASE – membuat database baru


2. USE DATABASE – memilih database aktif


3. CREATE TABLE – membuat tabel beserta struktur kolom


4. PRIMARY KEY & FOREIGN KEY – mendefinisikan hubungan antar tabel


5. NOT NULL, DEFAULT, AUTO_INCREMENT – memberi aturan data



Contoh Perintah:

CREATE DATABASE order_entry;
USE order_entry;

CREATE TABLE customers (
    cust_id CHAR(5) PRIMARY KEY,
    cust_name VARCHAR(50) NOT NULL,
    cust_address VARCHAR(100)
);

Tujuan BAB 3:

✔ Mampu membuat database dan tabel dari awal
✔ Memahami struktur tabel & tipe data
✔ Mampu menerapkan relasi antar tabel


---

📍 BAB 4 — Data Definition Language (DDL) Lanjutan

Topik Utama:

1. ALTER TABLE – mengubah struktur tabel


2. MODIFY – mengubah tipe data kolom


3. CHANGE – mengubah nama kolom


4. ADD / DROP COLUMN – menambah & menghapus kolom


5. RENAME TABLE – memberi nama baru pada tabel


6. DROP TABLE – menghapus tabel sepenuhnya



Contoh Perintah:

ALTER TABLE customers
ADD cust_status VARCHAR(10);

ALTER TABLE customers
CHANGE cust_contact kontak VARCHAR(50);

ALTER TABLE customers
DROP COLUMN cust_email;

RENAME TABLE customers TO customer_new;

DROP TABLE contact_customer;

Tujuan BAB 4:

✔ Memahami cara memodifikasi tabel tanpa menghapusnya
✔ Dapat menambah/menghapus/ubah kolom
✔ Mampu menghapus & mengganti nama tabel


---

📍 BAB 5 — Data Manipulation Language (DML)

Topik Utama:

1. INSERT – memasukkan data


2. SELECT – mengambil/menampilkan data


3. UPDATE – mengubah data


4. DELETE – menghapus data


5. WHERE – filter berdasarkan kondisi


6. Operator relasional (=, <, >, <=, >=, !=, OR, AND)



Contoh Perintah:

-- INSERT
INSERT INTO customers VALUES ('10000', 'Coyote Inc.', 'Arizona');

-- SELECT
SELECT * FROM products WHERE prod_price > 20;

-- UPDATE
UPDATE customers
SET cust_country = 'IND'
WHERE cust_id = '10002';

-- DELETE
DELETE FROM mahasiswa WHERE NIM = '00002682';

Tujuan BAB 5:

✔ Mampu mengisi data ke dalam tabel Order Entry
✔ Mampu menampilkan data dengan berbagai kondisi
✔ Mengubah dan menghapus data dengan aman
✔ Menguasai dasar query SQL (SELECT, WHERE, AND, OR, dll.)


---

📂 Output Laporan Tiap BAB (Bab 3, 4, 5)

Format file:

PrakDB_Bab3-NIM.odt

PrakDB_Bab4-NIM.odt

PrakDB_Bab5-NIM.odt


Isi laporan:

1. Source Code SQL


2. Screenshot hasil eksekusi / CMD


3. Disimpan di folder: PrakDB-NIM/




---

📌 Kesimpulan Umum

BAB 3 fokus membangun struktur database

BAB 4 fokus mengubah struktur database

BAB 5 fokus memanipulasi isi data dalam tabel


Tiga bab ini menjadi fondasi utama memahami SQL sebelum masuk ke join, aggregation, dan subquery pada bab berikutnya.
