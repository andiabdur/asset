# Managing Kubesphare Ks Core & Install Kubernetes

🔑 **Solution [here](https://github.com/andiabdur/asset)**  

---

# 📦 Dependency Requirements

KubeKey dapat menginstal **Kubernetes** dan **KubeSphere** secara bersamaan.  
Beberapa dependency harus sudah terpasang sebelum instalasi Kubernetes versi ≥ **1.18**.  

Silakan cek tabel berikut untuk memastikan dependensi sudah ada di node kamu:  

| Dependency | Kubernetes Version ≥ 1.18 |
|------------|----------------------------|
| `socat`    | Required                   |
| `conntrack`| Required                   |
| `ebtables` | Optional but recommended   |
| `ipset`    | Optional but recommended   |
| `ipvsadm`  | Optional but recommended   |

---

### atau bisa menjalankan dibawah ini agar lebih mempermudah saat installasinya

``` bash
sudo apt install socat conntrack ipvsadm -y

```

# Install Kubernetes Menggunakan Kubekey 

### ⌛️ Download Kubekey menggunakan Command Dibawah ini 

``` bash
curl -sfL https://get-kk.kubesphere.io | sh -

```
### ⏰ Proscess Membuat File config-v1.33.1.yaml menggunakan Kubekey Berikut Commandnya

``` bash
./kk create config [--with-kubernetes version] [(-f | --filename) path]
```

- Jika Sudah Terbuat untuk file confignya bisa Edit file confignya dan sesuaikan dengan node yang sudah ada

### 🚀 Setelah Kalian Edit dan simpan kalian bisa menjalankan script berikut ini di command kalian

``` bash
./kk create cluster -f [(-f | --filename) path]

```

# ▶️ Untuk Install Kubesphare Bisa menggunakan Command Dibawah Ini

```bash

curl -sSL https://raw.githubusercontent.com/andiabdur/asset/refs/heads/main/install-kubesphere.sh | bash

```
