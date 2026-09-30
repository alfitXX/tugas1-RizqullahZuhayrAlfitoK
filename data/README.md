# Data Tugas 1

## Dataset yang Dipilih

Isi informasi berikut sebelum Milestone 1.

| Item | Isi |
|---|---|
| Nama dataset | `[isi nama dataset]` |
| Sumber | `[URL BPS / Satu Data Indonesia / BMKG / HuggingFace / Kaggle]` |
| Lisensi/ketentuan pakai | `[isi]` |
| Ukuran | `[>= 500 MB atau > 1.000.000 baris]` |
| Periode data | `[isi]` |
| Unit analisis | `[isi]` |

## Tempat Mencari Dataset

Pilih dataset Indonesia yang legal digunakan, dapat didokumentasikan sumbernya, dan memenuhi batas ukuran tugas.

| Situs | Kegunaan |
|---|---|
| [Satu Data Indonesia](https://data.go.id/) | Portal data terbuka lintas instansi pemerintah Indonesia. |
| [Badan Pusat Statistik](https://www.bps.go.id/) | Statistik sosial, ekonomi, kependudukan, dan data wilayah. |
| [BMKG Data Online](https://dataonline.bmkg.go.id/) | Data cuaca, iklim, gempa bumi, dan observasi meteorologi. |
| [Hugging Face Datasets](https://huggingface.co/datasets) | Dataset publik yang dapat dicari berdasarkan topik, bahasa, atau ukuran. |
| [Kaggle Datasets](https://www.kaggle.com/datasets) | Katalog dataset publik; periksa lisensi dan dokumentasi pembuatnya. |
| [Google Dataset Search](https://datasetsearch.research.google.com/) | Mesin pencari untuk menemukan dataset dari berbagai portal. |

## Cara Memperoleh Data

1. Buka URL sumber di atas.
2. Unduh file ke folder `data/raw/` tanpa mengubah data mentah.
3. Catat nama file dan checksum bila tersedia.
4. Ubah variabel `DATA_PATH` pada `notebooks/01_data_profiling.ipynb` agar menunjuk ke file tersebut.

## Aturan Penyimpanan

- Jangan commit dataset mentah atau hasil olahan berukuran besar ke Git.
- File pada `data/raw/` adalah data asli dan tidak boleh diubah.
- Simpan hasil transformasi yang dapat direproduksi pada `data/processed/`.


# Data Tugas 1

## Dataset yang Dipilih

Isi informasi berikut sebelum Milestone 1.

| Item | Isi |
|---|---|
| Nama dataset | Indonesian News Dataset (`indonesian_news_dataset`), gabungan artikel dari 7 portal berita Indonesia |
| Sumber | [Kaggle: iqbalmaulana/indonesian-news-dataset](https://www.kaggle.com/datasets/iqbalmaulana/indonesian-news-dataset) |
| Lisensi/ketentuan pakai | Mengikuti ketentuan pada halaman Kaggle (bagian *License*, **perlu dicek ulang sebelum Milestone 1**). Dipakai hanya untuk keperluan akademik/non-komersial. Isi artikel bersumber dari Tempo, CNN Indonesia, CNBC Indonesia, Okezone, Suara, Kumparan, dan JawaPos, sehingga hak cipta tetap dimiliki masing-masing portal dan sumbernya wajib dicantumkan. |
| Ukuran | 737,92 MB (`data.csv`, setelah diekstrak; unduhan zip sekitar 285 MB). Memenuhi batas >= 500 MB. Jumlah baris akan dicatat setelah data profiling. |
| Periode data | 10 Agustus 2018 sampai 11 April 2023 (mayoritas data terkonsentrasi pada Maret sampai April 2023) |
| Unit analisis | Satu artikel berita per baris, dengan kolom waktu `created_at` (dan `updated_at`) |

## Tempat Mencari Dataset

Pilih dataset Indonesia yang legal digunakan, dapat didokumentasikan sumbernya, dan memenuhi batas ukuran tugas.

| Situs | Kegunaan |
|---|---|
| [Satu Data Indonesia](https://data.go.id/) | Portal data terbuka lintas instansi pemerintah Indonesia. |
| [Badan Pusat Statistik](https://www.bps.go.id/) | Statistik sosial, ekonomi, kependudukan, dan data wilayah. |
| [BMKG Data Online](https://dataonline.bmkg.go.id/) | Data cuaca, iklim, gempa bumi, dan observasi meteorologi. |
| [Hugging Face Datasets](https://huggingface.co/datasets) | Dataset publik yang dapat dicari berdasarkan topik, bahasa, atau ukuran. |
| [Kaggle Datasets](https://www.kaggle.com/datasets) | Katalog dataset publik; periksa lisensi dan dokumentasi pembuatnya. |
| [Google Dataset Search](https://datasetsearch.research.google.com/) | Mesin pencari untuk menemukan dataset dari berbagai portal. |

## Cara Memperoleh Data

1. Buka URL sumber di atas: <https://www.kaggle.com/datasets/iqbalmaulana/indonesian-news-dataset> (perlu login Kaggle).
2. Unduh file ke folder `data/raw/` tanpa mengubah data mentah. Via CLI:

```bash
   kaggle datasets download -d iqbalmaulana/indonesian-news-dataset -p data/raw/ --unzip
```

   Atau unduh langsung: <https://www.kaggle.com/api/v1/datasets/download/iqbalmaulana/indonesian-news-dataset>
3. Catat nama file dan checksum bila tersedia. File yang diharapkan: `data/raw/data.csv`.

```bash
   sha256sum data/raw/data.csv
```

4. Ubah variabel `DATA_PATH` pada `notebooks/01_data_profiling.ipynb` agar menunjuk ke file tersebut:

```python
   DATA_PATH = "data/raw/data.csv"
```

## Aturan Penyimpanan

- Jangan commit dataset mentah atau hasil olahan berukuran besar ke Git.
- File pada `data/raw/` adalah data asli dan tidak boleh diubah.
- Simpan hasil transformasi yang dapat direproduksi pada `data/processed/`.