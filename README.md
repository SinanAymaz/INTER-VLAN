# Inter-VLAN Routing – Cisco Packet Tracer

##  Proje Hakkında

Bu proje, **Cisco Packet Tracer** üzerinde farklı VLAN'lar arasında iletişim sağlamak amacıyla **Inter-VLAN Routing** yapılandırmasını göstermektedir.

Router üzerinde **Router-on-a-Stick** yöntemi kullanılarak VLAN'lar arasında Layer 3 yönlendirme gerçekleştirilmiştir.

##  Proje Yapısı

* 1 Router
* 3 Switch
* PC ve Laptop cihazları
* VLAN 10 – AR-GE
* VLAN 20 – PAZARLAMA
* VLAN 30 – KİŞİSEL

##  IP Planı

| VLAN    | Departman | Network         | Gateway      |
| ------- | --------- | --------------- | ------------ |
| VLAN 10 | AR-GE     | 192.168.10.0/24 | 192.168.10.1 |
| VLAN 20 | PAZARLAMA | 192.168.20.0/24 | 192.168.20.1 |
| VLAN 30 | KİŞİSEL   | 192.168.30.0/24 | 192.168.30.1 |

##  Kullanılan Teknolojiler

* VLAN
* Access Port
* Trunk Port
* Router-on-a-Stick
* Inter-VLAN Routing
* IPv4
* Cisco IOS
* Cisco Packet Tracer

##  Projenin Amacı

Farklı VLAN'larda bulunan cihazların router üzerinden yönlendirilerek birbirleriyle iletişim kurmasını sağlamaktır.

Bu yapı sayesinde:

**VLAN 10 ↔ VLAN 20 ↔ VLAN 30**

arasında iletişim gerçekleştirilebilir.

##  Çalışma Mantığı

1. Switch'ler üzerinde VLAN 10, VLAN 20 ve VLAN 30 oluşturulmuştur.
2. Uç cihazlar ilgili VLAN'lara atanmıştır.
3. Switch'ler arasındaki bağlantılar **Trunk** olarak yapılandırılmıştır.
4. Router ile Switch arasındaki bağlantı Trunk olarak yapılandırılmıştır.
5. Router üzerinde her VLAN için bir subinterface oluşturulmuştur.
6. Her subinterface'e ilgili VLAN'ın gateway adresi verilmiştir.
7. Router, VLAN'lar arasındaki trafiği yönlendirmiştir.

##  Bağlantı Testi

VLAN'lar arasındaki iletişim **ping** komutu kullanılarak test edilmiştir.

Örnek:

```text
ping 192.168.20.x
ping 192.168.30.x
```

Başarılı ping sonucunda farklı VLAN'lardaki cihazların birbirleriyle iletişim kurabildiği doğrulanmıştır.

##  Öğrenilen Konular

* VLAN oluşturma
* VLAN'lara cihaz atama
* Access Port yapılandırması
* Trunk Port yapılandırması
* Router-on-a-Stick
* Inter-VLAN Routing
* IP adresleme
* Default Gateway yapılandırması
* Ping ile bağlantı testi


**Cisco Packet Tracer | Networking Lab | Inter-VLAN Routing**
