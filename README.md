# UPT TIK Undiksha

Repo ini merupakan kumpulan gist code Seminar Pengenalan Docker dan Kultur 
DevOps UPT TIK Universitas Pendidikan Ganesha 16 Desember 2020.

---

## 📄 Daftar Isi


<!-- vim-markdown-toc GFM -->

* [🌿 Installasi Git](#-installasi-git)
	* [🐧 Linux](#-linux)
	* [🍎 MacOS](#-macos)
	* [🏠 Windows](#-windows)
* [🐳 Installasi Docker](#-installasi-docker)
	* [🐧 Linux](#-linux-1)
	* [🍎 MacOS](#-macos-1)
	* [🏠 Windows](#-windows-1)
		* [Menggunakan Windows Subsystem for Linux 2](#menggunakan-windows-subsystem-for-linux-2)
* [👩‍💻 Text Editor Setup](#-text-editor-setup)
	* [Visual Studio Code](#visual-studio-code)
	* [(N)Vim](#nvim)
* [📝 Docker Cheatsheet](#-docker-cheatsheet)

<!-- vim-markdown-toc -->

## 🌿 Installasi Git

### 🐧 Linux

Git umumnya sudah terinstall secara default pada distro Linux. Anda bisa melakukan
instalasi Git pada distribusi Debian/Ubuntu dan turunannya dengan cara berikut:
1. Buka terminal emulator (Gnome Terminal atau Konsole)

2. Jalankan perintah berikut:

```
$ sudo apt update -y && sudo apt install git -y
```

### 🍎 MacOS

Pada sistem operasi MacOS Anda bisa menginstall Git dengan menggunakan Homebrew:

1. Buka Terminal emulator

2. Jalankan perintah berikut:


```console
$ brew install git
```

Jika Anda menggunakan distribusi selain Debian/Ubuntu atau turunannya, silahkan
sesuaikan dengan package manager dari distribusi tersebut.

### 🏠 Windows

Anda bisa mengunduh Git untuk windows melalui [link ini](https://git-scm.com/download/win).

--- 


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


### 🏠 Windows 

Silahkan download Docker Desktop untuk Windows melalui [halaman ini](https://hub.docker.com/editions/community/docker-ce-desktop-windowsm).

#### Menggunakan Windows Subsystem for Linux 2

Jika Anda menggunakan Windows 10 versi 2004 Anda bisa menikmati integraasi Docker dengan
Windows Subsystem for Linux 2. Ikuti langkah-langkah berikut untuk mengaktifkan WSL2.

1. Aktifkan Windows Subsystem for Linux. Buka **Powershell** sebagai (Open as Administrator) 
Administrator dan jalankan perintah berikut:

```console
> dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

2. Aktifkan fitur **Virtual Machine Platform**:

```console
> dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

3. Update Linux kernel dengan mengunduh dari [halaman berikut](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi).
4. Aktifkan WSL2 sebagai default. Buka **Powershell** sebagai Administrator 
(Open as Administrator) dan jalankan perintah berikut:

```console
> wsl --set-default-version 2
```

5. Install salah satu distribusi Linux yang Anda inginkan melalui [Microsoft Store](https://aka.ms/wslstore) .
Untuk pemula saya merekomendasikan Anda menggunakan [Ubuntu](https://aka.ms/wslstore).
6. Install Windows Terminal dan jalankan distribusi Linux yang Anda sudah Anda install.
7. Ikuti kembali langkah instalasi Docker pada sistem operasi Linux di atas.

---

## 👩‍💻 Text Editor Setup

### Visual Studio Code

Text editor paling mudah dan kaya fitur yang bisa Anda gunakan adalah Visual
Studio Code. Install Visual Studio Code sesuai dengan sistem operasi yang Anda gunakan 
melalui [link berikut](https://code.visualstudio.com/download).

Lanjutkan dengan menginstall plugin Visual Studio Code berikut  ini:
1. [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
Plugin untuk memudahkan penggunaan Git.
2. [YAML](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml)
Anda akan memerlukan plugin ini saat bekerja dengan YAML file.
3. [Docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)
Hampir sama dengan Docker Desktop.
4. [Remote - WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)
Untuk bekerja dengan Docker dalam WSL
5. [Remote - SSH](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh)
Untuk bekerja dengan remote code via SSH  

### (N)Vim

Vim adalah text editor yang sangat cocok digunakan untuk mengedit configuration 
file. Sebagai opsi, saya sangat menyarankan Anda menginsall [CoC.nvim](https://github.com/neoclide/coc.nvim) 
dengan extentsion berikut:

1. coc-yaml
2. coc-docker
3. coc-git

---

## 📝 Docker Cheatsheet

Menampilkan daftar image
```console
$ docker images ls
```

Menampilkan daftar container yang sedang berjalan.
```console
$ docker container ls
```

Menampilkan semua container dalam registry
```console
$ docker container ls -a
```


