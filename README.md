
# 🚀 Go Project Template
Template ini adalah starter project untuk aplikasi Golang dengan struktur yang sudah tertata berdasarkan Clean Architecture. Template ini bisa digunakan sebagai dasar untuk membangun aplikasi baru tanpa perlu mengatur struktur dari nol.

## 📂 Struktur Direktori

```
project-root/
│── cmd/
│   └── your-app/
│       └── main.go          # Entry point aplikasi
│
│── internal/
│   ├── app/
│   │   ├── handler/         # Layer handler (HTTP layer)
│   │   │   ├── user_handler.go
│   │   │   ├── response.go
│   │   ├── service/         # Layer service (Business logic)
│   │   │   ├── user_service.go
│   ├── domain/
│   │   ├── model/           # Model entity
│   │   │   ├── user.go
│   │   ├── repository/      # Repository layer (Data access)
│   │   │   ├── user_repository.go
│
│── pkg/
│   ├── db/                  # Database setup & migration
│   │   ├── database.go
│   │   ├── migration.go
│   ├── config/              # Konfigurasi
│   │   ├── config.go
│
│── api/                     # API documentation (Swagger)
│
│── web/                     # Jika ingin menambahkan UI
│
│── scripts/                 # Untuk script otomatisasi
│
│── configs/                 # File konfigurasi seperti .env
│
│── tests/                   # Unit & integration tests
│
│── docs/                    # Dokumentasi
│
│── go.mod                    # Go module file
│── go.sum                    # Dependency file
```
## 🚀 Cara Menggunakan Template Ini
### 1️⃣ Clone Repository
Karena ini template, kamu bisa membuat repository baru di GitHub dan menggunakan template ini:

* Di GitHub:

Clone template ini secara manual:
```
git clone https://github.com/username/repo-template.git my-new-project
cd my-new-project
rm -rf .git  # Hapus riwayat Git agar menjadi proyek baru
git init     # Inisialisasi repository baru
```

### 2️⃣ Inisialisasi Go Module
Jalankan perintah berikut untuk menginisialisasi proyek baru:
```
go mod init yourusername/my-new-project
go mod tidy
```
Gantilah ```yourusername/my-new-project``` dengan nama module yang sesuai.

## 📌 Next Steps
Sesuaikan struktur proyek sesuai kebutuhan aplikasimu.
Tambahkan dependensi yang diperlukan dengan go get.
Mulai mengembangkan fitur aplikasi di dalam direktori internal/.
Buat dan jalankan testing di dalam direktori tests/.
Deploy proyekmu dengan membangun binary atau menggunakan container.

## 📄 Lisensi
Template ini menggunakan lisensi MIT, jadi kamu bebas menggunakannya untuk proyek pribadi maupun komersial.

