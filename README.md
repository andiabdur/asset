# Install Kubernetes & Kubespheree

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


### atau bisa menjalankan dibawah ini agar lebih mempermudah saat installasinya

``` bash
sudo apt install socat conntrack ipvsadm -y
```

---

# ⌛️ Install Kubernetes Menggunakan Kubekey 

``` bash
curl -O https://raw.githubusercontent.com/andiabdur/asset/main/install-kubekey.sh

chmod +x install-kubekey.sh

./install-kubesphere.sh
```

---


# ▶️ Install Kubesphare 

```bash

curl -sSL https://raw.githubusercontent.com/andiabdur/asset/refs/heads/main/install-kubesphere.sh | bash

```
