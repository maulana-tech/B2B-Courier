# B2B Courier Analysis | Analisis Kurir B2B

[English](#english) | [Bahasa Indonesia](#bahasa-indonesia)

# English

## Project Overview
This project analyzes courier service charges and billing discrepancies for a B2B (Business-to-Business) courier operation. The analysis helps identify overcharging and undercharging instances by comparing expected charges with actual billed amounts.

## Data Sources
The project uses the following data files:
- `Order Report.csv` - Contains order details and SKU information
- `SKU Master.csv` - Contains product SKU and weight information
- `pincodes.csv` - Maps warehouse and customer pincodes to delivery zones
- `Courier Company - Rates.csv` - Contains courier company rate cards for different zones
- `Invoice.csv` - Contains actual billing information from the courier company

## Analysis Components
1. **Data Preprocessing**
   - Removal of unnecessary columns
   - Merging of relevant datasets
   - Weight conversion from grams to kilograms
   - Weight slab calculation

2. **Charge Calculation**
   - Expected charge calculation based on:
     - Delivery zones
     - Weight slabs
     - Shipment types (Forward/RTO)
   - Comparison with actual billed amounts

3. **Discrepancy Analysis**
   - Identification of correctly charged orders
   - Detection of overcharged orders
   - Detection of undercharged orders
   - Calculation of total discrepancy amounts

## Key Findings
The analysis revealed:
- 12 orders were correctly charged
- 382 orders were overcharged (Total overcharge: Rs. 33,750.5)
- 7 orders were undercharged (Total undercharge: Rs. -165.2)

## Visualization
The project includes a pie chart visualization showing the proportion of correctly charged, overcharged, and undercharged orders.

## Dependencies
- Python 3.x
- Pandas
- Plotly

## Usage
1. Ensure all data files are in the same directory as the notebook
2. Install required dependencies
3. Run the Jupyter notebook `B2B_Courier.ipynb`

---

# Bahasa Indonesia

## Gambaran Proyek
Proyek ini menganalisis biaya layanan kurir dan perbedaan penagihan untuk operasi kurir B2B (Business-to-Business). Analisis ini membantu mengidentifikasi kasus kelebihan dan kekurangan penagihan dengan membandingkan biaya yang diharapkan dengan jumlah yang sebenarnya ditagih.

## Sumber Data
Proyek ini menggunakan file data berikut:
- `Order Report.csv` - Berisi detail pesanan dan informasi SKU
- `SKU Master.csv` - Berisi informasi SKU dan berat produk
- `pincodes.csv` - Memetakan kode pos gudang dan pelanggan ke zona pengiriman
- `Courier Company - Rates.csv` - Berisi kartu tarif perusahaan kurir untuk berbagai zona
- `Invoice.csv` - Berisi informasi penagihan aktual dari perusahaan kurir

## Komponen Analisis
1. **Pra-pemrosesan Data**
   - Penghapusan kolom yang tidak diperlukan
   - Penggabungan dataset yang relevan
   - Konversi berat dari gram ke kilogram
   - Perhitungan slab berat

2. **Perhitungan Biaya**
   - Perhitungan biaya yang diharapkan berdasarkan:
     - Zona pengiriman
     - Slab berat
     - Jenis pengiriman (Forward/RTO)
   - Perbandingan dengan jumlah yang ditagih sebenarnya

3. **Analisis Perbedaan**
   - Identifikasi pesanan yang ditagih dengan benar
   - Deteksi pesanan yang kelebihan tagihan
   - Deteksi pesanan yang kurang tagihan
   - Perhitungan total jumlah perbedaan

## Temuan Utama
Analisis mengungkapkan:
- 12 pesanan ditagih dengan benar
- 382 pesanan kelebihan tagihan (Total kelebihan: Rs. 33.750,5)
- 7 pesanan kurang tagihan (Total kekurangan: Rs. -165,2)

## Visualisasi
Proyek ini mencakup visualisasi diagram lingkaran yang menunjukkan proporsi pesanan yang ditagih dengan benar, kelebihan tagihan, dan kurang tagihan.

## Dependensi
- Python 3.x
- Pandas
- Plotly

## Penggunaan
1. Pastikan semua file data berada dalam direktori yang sama dengan notebook
2. Instal dependensi yang diperlukan
3. Jalankan Jupyter notebook `B2B_Courier.ipynb`

## Penulis
Maulana

## Lisensi
Proyek ini dilisensikan di bawah Lisensi MIT - lihat file LICENSE untuk detailnya.