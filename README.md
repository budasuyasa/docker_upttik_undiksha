# UPT TIK Undiksha

Repo ini merupakan kumpulan gist code Seminar Pengenalan Docker dan Kultur 
DevOps UPT TIK Universitas Pendidikan Ganesha 16 Desember 2020.


## 🐳 Installasi Docker

Silahkan pilih salah satu metode instalasi di bawah sesesua dengan sistem operasi
dan tools yang familiar dengan Anda.

### 🐧 Linux

Ikutilah langkah langkah berikut untuk menginstall Docker Engine pada sistem operasi
berbasis Linux.

1. Unduh script installer Docker Engine. Script ini akan secara otomatis mendeteksi
jenis dan package manager dari distribusi Linux yang Anda gunakan.

```console
$ curl -fsSL https://get.docker.com -o get-docker.sh
$ sudo sh get-docker.sh
```


### 🍎 MacOS

Docker tersedia untuk sistem operasi MacOs, Anda bisa Anda bisa mengunduuh
Docker untuk MacOS pada halaman [berikut ini](https://hub.docker.com/editions/community/docker-ce-desktop-macm).


### 🗔 Windows 

Silahkan download Docker untuk Windows melalui [halaman](https://hub.docker.com/editions/community/docker-ce-desktop-windowsm).

#### Menggunakan Windows Subsystem for Linux 2

Jika Anda menggunakan Windows 10 versi 2004 Anda bisa menikmati integraasi Docker dengan
Windows Subsystem for Linux 2. Ikuti langkah-langkah berikut untuk mengaktifkan WSL2.

1. Aktifkan Windows Subsystem for Linux. Buka **Powershell** sebagai (Open as Administrator) 
Administrator dan jalankan perintah berikut:

```console
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

2. Aktifkan fitur **Virtual Machine Platform**:

```console
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

3. Update Linux kernel dengan mengunduh dari [halaman berikut](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi).

4. Aktifkan WSL2 sebagai default. Buka **Powershell** sebagai Administrator 
(Open as Administrator) dan jalankan perintah berikut:

```console
wsl --set-default-version 2
```

5. Install salah satu distribusi Linux yang Anda inginkan melalui [Microsoft Store](https://aka.ms/wslstore) .
Untuk pemula saya merekomendasikan Anda menggunakan [Ubuntu](https://aka.ms/wslstore).

6. Install Windows Terminal dan jalankan distribusi Linux yang Anda sudah Anda install.

7. Ikuti kembali langkah instalasi Docker pada sistem operasi Linux di atas.

