# Literature GAP Matrix & Usulan Paper Kelompok
**Domain:** Patroli Siber, Deteksi Konten Radikal/Ekstremis, dan RAG Intelijen  
**NIM / Peneliti:** P36.2026.00024  
**Repository GitHub:** https://github.com/p36202600024-coder/S2-AI-RAG  

---

## 1. Literature GAP Matrix

| No | Penulis & Tahun | Judul Penelitian | Metode AI / RAG | Fokus Konten / Domain | Temuan Utama | Research Gap / Keterbatasan |
|---|---|---|---|---|---|---|
| **1** | Berte, S. (2025) | *Retrieval-Augmented Social Media Intelligence* | RAG + LLM + OSINT Crawling (Cheshire Cat AI) | Radikalisme, Terorisme, & Ujaran Kebencian di X | RAG meningkatkan akurasi deteksi narasi propaganda berdasarkan *knowledge base* analisis psikologi & siber. | Berfokus pada teks statis platform X; belum mendukung analisis multimodal (gambar/video) dan dialek/slang lokal. |
| **2** | Rahman et al. (2024) | *Retrieval Augmented Generation for Robust Cyber Defense* | Knowledge Graph RAG (KG-RAG) + Neo4j | Ancaman Siber, Propaganda Taktis, & Pemetaan Jaringan | Integrasi Graph DB berhasil menekan angka halusinasi LLM dalam pemetaan relasi antar-entitas ancaman siber. | *Overhead* pembuatan Knowledge Graph tinggi; belum dioptimalkan untuk respons otomatis *real-time streaming* dari patroli siber. |
| **3** | Bussari, S. (2025) | *RAGSec: RAG for Cybersecurity Threat Intelligence* | Standard Vector RAG + Dense Retrieval | Teks Ancaman & Pesan Bahaya Jaringan | Mempercepat *threat classification* hingga 60% dibanding model *classifier* NLP tradisional. | Kinerja pencarian *vector database* mengalami penurunan ketepatan (*latency issue*) pada arus data *cyber surveillance* yang masif. |
| **4** | Stephens, N. R. (2026) | *LLM-Enhanced OSINT and Cyberterrorism Detection* | LLM + Hybrid Sparse-Dense RAG | Ekstremisme & *Linguistic Markers* Radikal | Berhasil mengidentifikasi pola bahasa terselubung dan narasi radikal ekstremis dengan presisi tinggi. | Rentan terhadap manipulasi teks (*adversarial prompt/code-switching*) serta kurangnya konteks intelijen spesifik wilayah/negara tertentu. |

---

## 2. Analisis Research Gap & Usulan Paper Kelompok

### Analisis Research Gap
Berdasarkan sintesis yang dihasilkan oleh *pipeline* RAG di atas, ditemukan 3 keterbatasan utama pada penelitian saat ini:
1. **Unimodal vs Multimodal:** Sebagian besar sistem RAG patroli siber yang ada saat ini hanya memproses teks tunggal (*unimodal*), sedangkan propaganda radikal dan konten ekstremis berkembang pesat menggunakan poster, *meme*, video pendek, dan transkrip audio.
2. **Konteks Lokal dan Bahasa Terselubung:** Sistem RAG global belum mampu memahami idiom lokal Bahasa Indonesia, bahasa gaul, akronim terselubung, serta istilah khusus yang digunakan sel-sel radikal lokal untuk mengelabui *keyword filter*.
3. **Integrasi Alur Kerja Operasional Intelijen:** Penelitian terdahulu masih berdiri sendiri sebagai alat *standalone* dan belum diintegrasikan langsung ke dalam alur kerja pelaporan intelijen berjenjang (seperti alur Case Officer, Ketua Tim, Kasubdit, hingga penginputan otomatis ke dalam database/Aplikasi PASTI).

### Usulan Paper Kelompok
* **Judul Usulan:**  
  > **"Pengembangan Multimodal Agentic-RAG Terintegrasi Knowledge Graph untuk Patroli Siber dan Otomatisasi Alur Kerja Pelaporan Intelijen Radikalisme"**

* **Novelty & Solusi yang Ditawarkan:**
  * **Multimodal Agentic RAG:** Mengembangkan arsitektur RAG yang menggunakan *Agentic Workflow* untuk mengekstrak informasi dari teks, poster, maupun gambar propaganda secara otomatis.
  * **Hybrid Knowledge Graph Lintas Entitas:** Mengintegrasikan *Vector Search* dengan *Knowledge Graph* (KG) yang menyimpan taksonomi radikalisme lokal Indonesia guna memetakan hubungan antar-target (*Cyber Surveillance* dan *Covert*) secara akurat tanpa risiko halusinasi.
  * **Otomatisasi Alur Pelaporan Subdit Intelijen:** Mengintegrasikan luaran RAG langsung ke dalam format laporan berjenjang (Draft Lap LI, Lap Perkembangan, Lap Pemetaan Jaringan, hingga ringkasan eksekutif Lap Kirpat/Lap Situasi) untuk mempercepat verifikasi Katim/Kasubdit serta mengeliminasi *manual input* pada Aplikasi PASTI.
