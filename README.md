Inter-VLAN Routing – Cisco Packet Tracer
Bu proje, Cisco Packet Tracer üzerinde farklı VLAN'ların yapılandırılması ve router üzerinden birbirleriyle haberleştirilmesini göstermektedir.
Proje Yapısı
    • VLAN 10 – AR-GE → 192.168.10.0/24
    • VLAN 20 – PAZARLAMA → 192.168.20.0/24
    • VLAN 30 – PERSONEL → 192.168.30.0/24
    • 1 Router
    • 3 Switch
    • PC ve Laptop istemciler
    • Switchler arasında trunk bağlantıları
    • Router ile Inter-VLAN Routing
Amaç
Farklı VLAN'larda bulunan cihazların, Inter-VLAN Routing kullanılarak birbirleriyle iletişim kurmasını sağlamak.
Kullanılan Teknolojiler
    • VLAN
    • Access Port
    • Trunk Port
    • Router-on-a-Stick
    • Inter-VLAN Routing
    • IPv4
    • Cisco IOS
    • Cisco Packet Tracer
IP Planı
VLAN
Departman
Network
10
AR-GE
192.168.10.0/24
20
PAZARLAMA
192.168.20.0/24
30
PERSONEL
192.168.30.0/24
Gateway'ler
    • VLAN 10 → 192.168.10.1
    • VLAN 20 → 192.168.20.1
    • VLAN 30 → 192.168.30.1
Projenin Çalışma Mantığı
İstemci cihazlar ilgili VLAN'lara atanır. Switchler arasındaki bağlantılar trunk olarak yapılandırılır. Router üzerindeki alt arayüzler ise VLAN'ların gateway görevini üstlenir.
Böylece VLAN 10, VLAN 20 ve VLAN 30 arasında Layer 3 yönlendirme gerçekleştirilerek cihazların birbirleriyle iletişim kurması sağlanır.
Test
Bağlantının çalıştığını doğrulamak için istemciler arasında:
ping 192.168.20.x
ping 192.168.30.x
gibi ping testleri yapılabilir.
Öğrenilen Konular
Bu proje ile:
    • VLAN oluşturma
    • VLAN'lara cihaz atama
    • Access port yapılandırma
    • Trunk yapılandırma
    • Router-on-a-Stick
    • Inter-VLAN Routing
    • IP adresleme
    • Gateway yapılandırması
    • Ping ile bağlantı testi
konularında pratik yapılmıştır.
