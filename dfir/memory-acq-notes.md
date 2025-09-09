# 🧠 DFIR – Memory & Disk Acquisition Notes

Guidelines for acquiring **volatile (RAM)** and **non-volatile (disk)** data in incident response.  
Focus: **forensic soundness** and **chain of custody**.

---

## 💻 Memory Acquisition (RAM)
- [ ] Use trusted tools: `FTK Imager`, `Belkasoft RAM Capturer`, `DumpIt`, `WinPMEM`  
- [ ] Save image in raw format (`.raw`, `.bin`)  
- [ ] Calculate hash (MD5/SHA256) immediately after acquisition  
- [ ] Document environment: hostname, time, user logged in  

**Linux Example:**
sudo LiME -o /mnt/usb/memdump.raw -f raw
sha256sum memdump.raw > memdump.raw.sha256

---

## 💽 Disk Acquisition
- [ ] Always use a write blocker (hardware or software)  
- [ ] Create a bit-by-bit copy (dd, FTK Imager, EnCase)  
- [ ] Save in `.E01` (EnCase format) or raw image  
- [ ] Verify image integrity with hashing  
- [ ] Record serial number, device type, acquisition time  

**Linux Example:**
sudo dd if=/dev/sda of=/mnt/usb/diskimage.dd bs=4M conv=noerror,sync
sha256sum diskimage.dd > diskimage.dd.sha256


---

## 🗂️ Chain of Custody
- Label evidence clearly (CaseID, Date, Collector)  
- Store in secure evidence locker / encrypted storage  
- Maintain documentation for legal admissibility  

---

# 🇹🇷 DFIR – Bellek & Disk Alma Notları

Olay müdahale sırasında **geçici (RAM)** ve **kalıcı (disk)** verilerin alınmasına dair rehber.  
Odak: **adli uygunluk** ve **delil zinciri**.

---

## 💻 Bellek (RAM) Alma
- [ ] Güvenilir araçlar kullan: `FTK Imager`, `Belkasoft RAM Capturer`, `DumpIt`, `WinPMEM`  
- [ ] İmajı raw formatta kaydet (`.raw`, `.bin`)  
- [ ] Hash değerini (MD5/SHA256) hemen hesapla  
- [ ] Sistem bilgilerini kaydet: hostname, zaman, kullanıcı  

**Linux Örnek:**
sudo LiME -o /mnt/usb/memdump.raw -f raw
sha256sum memdump.raw > memdump.raw.sha256


---

## 💽 Disk Alma
- [ ] Her zaman write blocker kullan (donanım veya yazılım)  
- [ ] Birebir kopya al (`dd`, FTK Imager, EnCase)  
- [ ] `.E01` veya raw format tercih et  
- [ ] Hash değerleriyle doğrula  
- [ ] Seri numarası, cihaz tipi, alma zamanı kaydedilmeli  

**Linux Örnek:**
sudo dd if=/dev/sda of=/mnt/usb/diskimage.dd bs=4M conv=noerror,sync
sha256sum diskimage.dd > diskimage.dd.sha256


---

## 🗂️ Delil Zinciri
- Delilleri net şekilde etiketle (CaseID, Tarih, Alan kişi)  
- Güvenli depoda / şifreli alanda sakla  
- Yasal geçerlilik için her adımı kaydet  

---

⚔️ *“If it’s not documented, it didn’t happen.”*








