# 🛡️ Incident Response – Triage Checklist

This document provides a **quick triage guide** for handling security incidents.  
Focus: **containment, evidence preservation, and rapid analysis.**

---

## 🔎 Host Triage (Endpoint)
- [ ] Isolate the machine from the network (disconnect / VLAN quarantine)  
- [ ] Acquire memory image (Volatility-compatible)  
- [ ] Collect system logs (Windows Event Logs / Syslog)  
- [ ] Gather running processes & network connections (`netstat`, `tasklist`, `pslist`)  
- [ ] Collect registry hives / config files  
- [ ] Secure disk image if necessary  

---

## 🌐 Network Triage
- [ ] Identify suspicious IPs, domains, traffic patterns  
- [ ] Check firewall/IDS/IPS logs for related alerts  
- [ ] Block malicious IPs/domains at perimeter devices  
- [ ] Capture live traffic if incident is ongoing (pcap with tcpdump/Wireshark)  
- [ ] Validate if attack is inbound, outbound, or lateral  

---

## 🗂️ Evidence Handling
- [ ] Use proper naming convention for evidence (timestamp, host, caseID)  
- [ ] Ensure evidence is write-protected and hashed (MD5/SHA256)  
- [ ] Document every action taken (who/what/when/where/why)  

---

## 📢 Communication & Reporting
- [ ] Notify incident response team / stakeholders  
- [ ] Escalate based on severity (critical, high, medium, low)  
- [ ] Prepare initial report with summary of findings  

---

# 🇹🇷 Olay Müdahale – Triage Kontrol Listesi

Bu doküman, güvenlik olaylarında **hızlı triage rehberi** sunar.  
Odak: **izolasyon, delil koruma ve hızlı analiz.**

---

## 🔎 Host Triage (Uç Nokta)
- [ ] Makineyi ağdan izole et (bağlantı kes / VLAN karantina)  
- [ ] Bellek imajı al (Volatility uyumlu)  
- [ ] Sistem loglarını topla (Windows Event Logs / Syslog)  
- [ ] Çalışan süreçler ve ağ bağlantılarını listele (`netstat`, `tasklist`, `pslist`)  
- [ ] Registry hives / konfigürasyon dosyalarını kaydet  
- [ ] Gerekirse disk imajı al  

---

## 🌐 Ağ Triage
- [ ] Şüpheli IP, domain ve trafik modellerini belirle  
- [ ] Firewall / IDS / IPS loglarını kontrol et  
- [ ] Kötü niyetli IP/domain’leri engelle  
- [ ] Olay devam ediyorsa canlı trafik kaydı al (pcap – tcpdump/Wireshark)  
- [ ] Saldırının yönünü belirle (gelen, giden, yatay hareket)  

---

## 🗂️ Delil Yönetimi
- [ ] Delilleri isimlendirme standardına göre kaydet (zaman, host, caseID)  
- [ ] Delilleri yazma korumalı sakla ve hash değerlerini al (MD5/SHA256)  
- [ ] Tüm adımları kaydet (kim/ne/ne zaman/nerede/niçin)  

---

## 📢 İletişim & Raporlama
- [ ] IR ekibini / paydaşları bilgilendir  
- [ ] Ciddiyetine göre eskale et (kritik, yüksek, orta, düşük)  
- [ ] İlk bulguları özetleyen rapor hazırla  

---

⚔️ *“Fast, precise, documented – triage defines the outcome of incident response.”*
