# Managing Kubesphare Ks Core & Install Kubernetes

🔑 **Solution [here](https://github.com/andiabdur/asset)**  

---

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
