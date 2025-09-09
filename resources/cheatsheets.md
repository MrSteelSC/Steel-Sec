# 📚 Cybersecurity Cheatsheets

Quick reference notes for common cybersecurity tasks.  
Designed for **fast recall during IR, Pentest, and DFIR**.

---

## 🔎 Nmap Essentials
nmap -T4 -F <target> # Fast scan
nmap -sV <target> # Service version detection
nmap -O <target> # OS detection
nmap -A <target> # Aggressive scan

---

## 🛡️ Common Linux Commands
ps aux # List processes
netstat -tulnp # Active network connections
lsof -i # Open sockets
journalctl -xe # System logs


---

## 🔐 Windows IR Quick Commands
Get-Process # Running processes
Get-Service # Services
Get-EventLog -LogName Security -Newest 20
netstat -ano # Network connections


---

## 🧩 Hashing & Verification
md5sum file.img
sha256sum file.img
certutil -hashfile file.img SHA256 # Windows

---

# 🇹🇷 Siber Güvenlik Cheat Sheet

Siber güvenlikte sık kullanılan komut ve notlar.  
Odak: **IR, Pentest, DFIR sırasında hızlı erişim**.

---

## 🔎 Nmap Temel Komutlar
nmap -T4 -F <hedef> # Hızlı tarama
nmap -sV <hedef> # Servis & versiyon tespiti
nmap -O <hedef> # İşletim sistemi tespiti
nmap -A <hedef> # Agresif tarama

---

## 🛡️ Linux Temel Komutlar
ps aux # Süreçleri listele
netstat -tulnp # Aktif bağlantılar
lsof -i # Açık soketler
journalctl -xe # Sistem logları


---

## 🔐 Windows IR Komutları
Get-Process # Çalışan süreçler
Get-Service # Servisler
Get-EventLog -LogName Security -Newest 20 # Güvenlik logları
netstat -ano # Ağ bağlantıları


---

## 🧩 Hash & Doğrulama
md5sum file.img
sha256sum file.img
certutil -hashfile file.img SHA256 # Windows için


---

⚔️ *“Cheat sheets are not shortcuts, they’re survival kits.”*
















