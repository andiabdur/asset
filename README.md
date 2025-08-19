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

# 🌐 Networking & DNS Requirements

- Pastikan DNS address di file `/etc/resolv.conf` tersedia.  
  Jika tidak, bisa menyebabkan masalah DNS di cluster.  

- Jika konfigurasi network kamu menggunakan **Firewall** atau **Security Group**,  
  pastikan semua komponen infrastruktur bisa saling berkomunikasi melalui port tertentu.  

# Install Kubernetes Menggunakan Kubekey 

## ⌛️ Download Kubekey menggunakan Command Dibawah ini 

``` bash
curl -sfL https://get-kk.kubesphere.io | sh -

```
## ⏰ Proscess Membuat File config-v1.33.1.yaml menggunakan Kubekey Berikut Commandnya

``` bash
./kk create config [--with-kubernetes version] [(-f | --filename) path]
```

- Jika Sudah Terbuat untuk file confignya bisa Edit file confignya dan sesuaikan dengan node yang sudah ada

## 🚀 Setelah Kalian Edit dan simpan kalian bisa menjalankan script berikut ini di command kalian

``` bash
./kk create cluster -f [(-f | --filename) path]

```

## ▶️ Run the following Commands in Your Terminal

```bash

curl -sSL https://raw.githubusercontent.com/andiabdur/asset/refs/heads/main/install-kubesphere.sh | bash

```
