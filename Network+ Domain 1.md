<div dir="rtl" align="right">

## 📚 **OSI Model – CompTIA Network+ (Objective 1.1)**

---

### 🧭 **تعريف**

نموذج **OSI (Open Systems Interconnection)** هو **إطار قياسي عالمي** يحدد كيف تتواصل الأنظمة الشبكية مع بعضها على سبع طبقات مترابطة.  
بدونه، لن تتمكن الأجهزة من فهم البيانات أو تبادلها بشكل منظم.

---

### 🔹 **الطبقات السبع في نموذج OSI (من الأدنى إلى الأعلى)**

|رقم|الطبقة|الاسم بالعربية|الوظيفة الأساسية|أمثلة|
|---|---|---|---|---|
|1️⃣|**Physical**|الفيزيائية|إرسال **البتات (Bits)** كإشارات كهربائية أو ضوئية عبر الوسيط.|كابلات UTP/Fiber، RJ45، Hubs، Repeaters|
|2️⃣|**Data Link**|رابط البيانات|تجميع البتات في إطارات (Frames)، كشف الأخطاء، عنونة MAC.|Switches|
|3️⃣|**Network**|الشبكة|عنونة IP، تحديد المسارات (Routing).|Routers، OSPF، BGP|
|4️⃣|**Transport**|النقل|تجزئة البيانات، التحكم بالتدفق، TCP/UDP.|TCP، UDP|
|5️⃣|**Session**|الجلسة|إدارة الجلسات بين الأنظمة.|Session Management، Authentication|
|6️⃣|**Presentation**|العرض|التشفير والضغط وتحويل الصيغ.|SSL/TLS، ASCII|
|7️⃣|**Application**|التطبيق|واجهة المستخدم للتفاعل مع الشبكة.|HTTP، SMTP، DNS، FTP|

---

### 🧠 **مثال توضيحي للتغليف (Encapsulation)**

|الطبقة|المهمة|التوضيح|
|---|---|---|
|7️⃣ Application|واجهة التطبيقات للمستخدم.|`https://mail.google.com`|
|6️⃣ Presentation|تشفير وتحويل البيانات.|SSL Encryption|
|5️⃣ Session|إدارة الجلسة بين الأجهزة.|Maintains connection|
|4️⃣ Transport|تغليف البيانات وتجزئتها.|TCP Segment|
|3️⃣ Network|إضافة العناوين المنطقية.|IP Packet|
|2️⃣ Data Link|إضافة عناوين MAC.|Ethernet Frame|
|1️⃣ Physical|إرسال الإشارات فعليًا.|Electrical/Optical signals|

---

### 📌 **الفرق بين OSI و TCP/IP**

|المعيار|عدد الطبقات|الاستخدام|
|---|---|---|
|**OSI Model**|7 طبقات|مرجع نظري لتفسير عمل الشبكات.|
|**TCP/IP Model**|4 طبقات (Application, Transport, Internet, Network Access)|النموذج العملي المستخدم فعليًا.|

---

#Network+

## 🧱 **Networking Devices – Objective 1.2**

---

### 🔹 **الأجهزة الفيزيائية والافتراضية (Networking Appliances)**

|الجهاز|الوظيفة|الطبقة / الملاحظات|
|---|---|---|
|**Router**|يربط الشبكات ويحدد أفضل مسار للبيانات.|Layer 3 – Network|
|**Switch**|يربط الأجهزة داخل LAN.|Layer 2 – Data Link (ويدعم L3 في السويتشات المُدارة).|
|**Firewall**|يفرض سياسات الأمان ويفلتر الترافيك.|L3/L4 تقليديًا – L7 في NGFW.|
|**IDS / IPS**|الكشف عن الهجمات (IDS) ومنعها (IPS).|تعمل عبر L3/L4/L7.|
|**Load Balancer**|توزيع الحمل على خوادم متعددة.|L4 أو L7|
|**Proxy Server**|وسيط لتخزين وفلترة البيانات.|L7 – Application Layer|
|**Access Point (AP)**|يربط الأجهزة اللاسلكية بالشبكة.|L2|
|**Wireless Controller**|إدارة مركزية لعدة نقاط وصول.|يستخدم في البيئات المؤسسية|
|**NAS / SAN**|تخزين عبر الشبكة.|NAS (LAN) – SAN (Data Center)|

---

### 🧩 **Networking Functions**

|الوظيفة|الهدف|المثال|
|---|---|---|
|**VPN**|تأمين الاتصال عبر نفق مشفر.|موظف يتصل بخوادم الشركة عن بُعد.|
|**QoS**|إدارة أولوية الترافيك.|VoIP أو بث الفيديو.|
|**TTL**|منع الحلقات عبر تحديد عمر الحزمة.|Ping/Traceroute.|

---

### 🌐 **Content Delivery Network (CDN)**

شبكة موزعة من خوادم الكاش لتسليم المحتوى من أقرب موقع للمستخدم، مما يقلل **الـLatency** ويحسن سرعة التحميل.  
**أمثلة:** Cloudflare, Akamai, Amazon CloudFront.

---

#Network+

## ☁️ **Cloud Concepts – Objective 1.8**

---

### 🟦 **مفاهيم أساسية**

|المفهوم|الوصف|
|---|---|
|**NFV**|تحويل وظائف الشبكة (مثل الراوتر والفايروال) إلى مكونات افتراضية.|
|**VPC**|شبكة خاصة افتراضية داخل السحابة العامة.|
|**Security Groups**|تشبه ACLs، تتحكم بالترافيك المسموح والمرفوض.|
|**VPN / Direct Connect**|اتصال آمن أو مباشر بين شركتك والسحابة.|

---

### ☁️ **نماذج النشر (Deployment Models)**

|النوع|الوصف|الاستخدام|
|---|---|---|
|**Public Cloud**|موارد مشتركة عبر الإنترنت.|AWS, Azure, GCP|
|**Private Cloud**|شبكة خاصة لمؤسسة واحدة.|البنوك، الجهات الحكومية|
|**Hybrid Cloud**|دمج بين العام والخاص.|توزيع الأحمال|
|**Community Cloud**|عدة منظمات تتشارك البنية.|الجامعات، المؤسسات البحثية|

---

### 🧩 **نماذج الخدمة (Service Models)**

|النموذج|الوصف|الأمثلة|
|---|---|---|
|**IaaS**|بنية تحتية كخدمة (سيرفرات، شبكات).|AWS EC2|
|**PaaS**|منصة تطوير وتشغيل التطبيقات.|Google App Engine|
|**SaaS**|برامج جاهزة عبر الإنترنت.|Gmail, Office 365|
|**XaaS**|أي خدمة تُقدَّم عبر الإنترنت.|Backup/Security as a Service|

---

### 📘 **VNIC (Virtual NIC)**

بطاقة شبكة افتراضية داخل الآلة الافتراضية (VM):  
تحتوي على **MAC Address + IP Address** وتربط الـVM بالـVPC Subnet.

---

### 🧠 **ملاحظات مهمة للامتحان**

- Public Cloud = أرخص وأقل أمانًا.
    
- Private Cloud = أغلى وأكثر أمانًا.
    
- Hybrid = مرن ومتوازن.
    
- **IaaS → تدير OS**
    
- **PaaS → تدير التطبيق فقط**
    
- **SaaS → تستخدمه جاهزًا بالكامل.**
---
## 🌐 **Protocols, Ports & Traffic Types – CompTIA Network+ (Objective 1.1 / 1.5)**

---

### 🔹 **البروتوكولات المهمة (Common Protocols)**

|البروتوكول|الاسم الكامل|الوظيفة الأساسية|
|---|---|---|
|**ICMP**|Internet Control Message Protocol|يُستخدم لاختبار الاتصال وتشخيص الأخطاء (مثل أوامر `ping` و `tracert`).|
|**TCP**|Transmission Control Protocol|بروتوكول موثوق (Connection-Oriented)، يضمن تسليم البيانات بالترتيب الصحيح.|
|**UDP**|User Datagram Protocol|بروتوكول غير موثوق (Connectionless)، أسرع، مناسب للبث ومكالمات الصوت.|
|**GRE**|Generic Routing Encapsulation|يُستخدم لإنشاء أنفاق VPN بسيطة داخل IP.|
|**IPSec**|Internet Protocol Security|يؤمن البيانات عبر التشفير والمصادقة في اتصالات VPN.|

---

### 🔹 **المنافذ الشائعة (Common Ports & Services)**

|الخدمة|المنفذ|البروتوكول|الوظيفة|
|---|---|---|---|
|**FTP**|20/21|TCP|نقل الملفات (غير مشفر).|
|**SFTP / SSH**|22|TCP|نقل آمن وإدارة عبر الطرفية.|
|**Telnet**|23|TCP|إدارة نصية للأجهزة (غير آمن).|
|**SMTP**|25|TCP|إرسال البريد الإلكتروني.|
|**DNS**|53|TCP / UDP|تحويل أسماء النطاقات إلى عناوين IP.|
|**DHCP**|67 / 68|UDP|توزيع عناوين IP تلقائيًا للعملاء.|
|**HTTP**|80|TCP|تصفح الويب (غير آمن).|
|**HTTPS**|443|TCP|تصفح الويب الآمن (SSL/TLS).|
|**NTP**|123|UDP|مزامنة الوقت بين الأجهزة.|
|**SNMP**|161 / 162|UDP|إدارة ومراقبة الشبكات.|
|**LDAP**|389|TCP / UDP|إدارة خدمات الأدلة (Directories).|
|**LDAPS**|636|TCP / UDP|إدارة الأدلة بشكل مشفر وآمن.|
|**RDP**|3389|TCP|التحكم بسطح المكتب عن بعد (Remote Desktop).|

---

### 🔹 **أنواع الترافيك (Traffic Types)**

|النوع|المعنى|الوصف|
|---|---|---|
|**Unicast**|واحد إلى واحد|الترافيك بين جهاز مرسل وجهاز مستلم محدد.|
|**Broadcast**|واحد إلى الكل|الترافيك يُرسل لكل الأجهزة في نفس الشبكة.|
|**Multicast**|واحد إلى مجموعة|يُرسل لمجموعة محددة من الأجهزة فقط.|
|**Anycast**|واحد إلى أقرب واحد|يُرسل إلى أقرب جهاز (أو خادم) من مجموعة متماثلة.|

---

### 📌 **الخلاصة للامتحان**

✅ **احفظ بدقة:**

- أرقام المنافذ الأساسية (SSH = 22, HTTPS = 443, RDP = 3389…).
    
- الفرق بين **TCP (موثوق)** و **UDP (سريع)**.
    
- أنواع الترافيك الأربعة (Uni / Broad / Multi / Anycast).
    
- **ICMP و IPSec و GRE** تأتي غالبًا في أسئلة سيناريوهات الشبكات.


---
## **Other Useful Protocols – Security & VPN (Objective 1.5 / 4.3)**

---

### 🔸 **IPSec (Internet Protocol Security)**

- يؤمّن الترافيك على **طبقة الشبكة (Layer 3)**.
    
- يُستخدم لإنشاء **VPNs**.
    
- يقدم الخصائص التالية:
    
    - **Confidentiality (السرية)**
        
    - **Integrity (سلامة البيانات)**
        
    - **Authentication (المصادقة)**
        
- يعتمد على بروتوكولات فرعية: **AH** و **ESP**.
    

---

### 📑 **AH (Authentication Header)**

- يوفر **التوثيق وسلامة البيانات** فقط.
    
- لا يقدّم **تشفيرًا** → لا يوجد Confidentiality.
    
- **Protocol Number: 51**
    

---

### 🔒 **ESP (Encapsulating Security Payload)**

- يوفر **التشفير + التوثيق + سلامة البيانات**.
    
- الأكثر استخدامًا في بيئات IPSec.
    
- **Protocol Number: 50**
    

---

### ⚙️ **IKE (Internet Key Exchange)**

- يُستخدم لتبادل المفاتيح وإنشاء **Security Association (SA)**.
    
- يعمل مع IPSec لبناء النفق الآمن.
    
- يتكوّن من مرحلتين:
    
    1. **Phase 1:** تبادل المفاتيح الآمنة.
        
    2. **Phase 2:** إنشاء النفق (Tunnel Establishment).
        

---

### 🛠 **Modes of IPSec**

|النمط|ما يتم تشفيره|الاستخدام|
|---|---|---|
|**Transport Mode**|فقط الـ Payload (البيانات) — IP Header يبقى واضحًا.|بين جهازين (Host-to-Host).|
|**Tunnel Mode**|كل الحزمة (Header + Payload).|بين شبكتين (Site-to-Site VPN).|

---

### 🌐 **VPN Types**

|النوع|الوصف|البروتوكولات الشائعة|
|---|---|---|
|**Site-to-Site VPN**|يربط شبكتين كاملتين عبر الإنترنت بنفق IPSec (Tunnel Mode).|IPSec|
|**Remote Access VPN**|اتصال مستخدم فردي بشبكة الشركة عن بعد.|SSL VPN / IPSec|

---

### 🌀 **GRE (Generic Routing Encapsulation)**

- بروتوكول نفق عام – **Protocol 47**.
    
- لا يوفّر تشفير أو حماية، فقط **تغليف (Encapsulation)**.
    
- يمكن دمجه مع IPSec لإضافة الأمان.
    

---

### 📡 **ICMP (Internet Control Message Protocol)**

- بروتوكول تشخيص — **Protocol 1**.
    
- يُستخدم في **ping** و **traceroute**.
    
- لا يحتوي على تشفير أو حماية، لكنه أساسي في مراقبة الشبكات.
    

---

### ✅ **خلاصة للمراجعة**

|البروتوكول / النمط|الوظيفة الأساسية|
|---|---|
|**IPSec**|تأمين الترافيك عبر Layer 3.|
|**AH**|توثيق فقط (بدون تشفير).|
|**ESP**|تشفير + توثيق.|
|**IKE**|تبادل المفاتيح وإنشاء SA.|
|**Transport Mode**|جهاز ↔ جهاز (Host-to-Host).|
|**Tunnel Mode**|شبكة ↔ شبكة (Site-to-Site).|
|**GRE**|تغليف بدون تشفير.|
|**ICMP**|تشخيص الاتصال (ping/traceroute).|


---

## 🧭 Network Communication Methods

### **1️⃣ Unicast**

- **Definition:** One-to-one communication.
    
- **Purpose:** Sends data **from one sender to one receiver**.
    
- **Example:** Browsing a website (client → server).
    
- **Analogy:** Sending a private letter to one address.
    

**Key point:**  
Efficient for specific communication, but not ideal for large groups.

---

### **2️⃣ Multicast**

- **Definition:** One-to-many communication, **only to a specific group**.
    
- **Purpose:** Sends data to **multiple selected recipients** who have joined a multicast group.
    
- **Example:** Streaming live events to multiple subscribers.
    
- **Analogy:** Like sending one copy of a letter to a club — only members get it.
    

**Key point:**  
Uses **Class D IP addresses (224.0.0.0–239.255.255.255)**.

---

### **3️⃣ Anycast**

- **Definition:** One-to-nearest communication.
    
- **Purpose:** Data is sent to **the closest (in routing terms)** of several possible receivers.
    
- **Example:** DNS root servers — your query reaches the nearest server.
    
- **Analogy:** Mailing a letter to “the nearest branch” of a global company.
    

**Key point:**  
Improves **performance and redundancy** by selecting the shortest network path.

---

### **4️⃣ Broadcast**

- **Definition:** One-to-all communication within a local network.
    
- **Purpose:** Sends data to **all devices on the subnet**.
    
- **Example:** ARP requests, DHCP Discover messages.
    
- **Analogy:** Announcing something over a loudspeaker — everyone nearby hears it.
    

**Key point:**  
Works only in **IPv4 networks** (IPv6 removed broadcast and uses multicast instead).

---

### 🔹 Quick Comparison Table

| Type      | Communication Style    | IPv4 Supported | IPv6 Supported | Example Use     |
| --------- | ---------------------- | -------------- | -------------- | --------------- |
| Unicast   | One to One             | ✅              | ✅              | Web browsing    |
| Multicast | One to Many (selected) | ✅              | ✅              | Video streaming |
| Anycast   | One to Nearest         | ⚠️ (rare)      | ✅              | DNS queries     |
| Broadcast | One to All             | ✅              | ❌              |                 |


---

# Wireless Networking - CompTIA Network+ N10-009 - 1.5
wireless standards , 802.11 networking , 
## 📶 IEEE 802.11 Standards (Wi-Fi Generations)

| **IEEE Standard** | **Generation Name** | **Frequencies**         | **Maximum Theoretical Link Rate** |
| ----------------- | ------------------- | ----------------------- | --------------------------------- |
| **802.11a**       | –                   | 5 GHz                   | 6 – 54 Mbit/s                     |
| **802.11b**       | –                   | 2.4 GHz                 | 1 – 11 Mbit/s                     |
| **802.11g**       | –                   | 2.4 GHz                 | 6 – 54 Mbit/s                     |
| **802.11n**       | **Wi-Fi 4**         | 2.4 GHz / 5 GHz         | 72 – 600 Mbit/s                   |
| **802.11ac**      | **Wi-Fi 5**         | 5 GHz                   | 433 – 6,933 Mbit/s                |
| **802.11ax**      | **Wi-Fi 6 / 6E**    | 2.4 GHz / 5 GHz / 6 GHz | 574 – 9,608 Mbit/s                |
| **802.11be**      | **Wi-Fi 7**         | 2.4 GHz / 5 GHz / 6 GHz | 1,376 – 46,120 Mbit/s             |
|                   |                     |                         |                                   |
|                   |                     |                         |                                   |



---

## 🔌 **Transceivers – CompTIA Network+ (Objective 1.5)**

---

### 🧭 **ما هو الـ Transceiver؟**

- كلمة **Transceiver** = **Transmitter + Receiver**.
    
- جهاز مسؤول عن **تحويل الإشارات الرقمية إلى ضوئية أو كهربائية والعكس**.
    
- يُستخدم لربط الأجهزة (مثل السويتش أو الراوتر) مع الوسيط المناسب — سواء **نحاسي أو ألياف ضوئية**.
    
- يُركّب في المنافذ القابلة للتبديل (Hot-swappable ports).
    

---

### ⚙️ **وظائف الـ Transceiver**

1. **الإرسال (Transmit):** تحويل البيانات من الجهاز إلى إشارة كهربائية أو ضوئية.
    
2. **الاستقبال (Receive):** استقبال الإشارة وتحويلها إلى بيانات رقمية مفهومة.
    
3. **المرونة:** يمكن استبداله بسهولة دون إيقاف الجهاز.
    
4. **التوافق:** يدعم وسائط مختلفة (Fiber / Copper).
    

---

### 🧩 **أنواع الـ Transceivers الشائعة**

|النوع|الاختصار|السرعة|الوسيط|المدى|الملاحظات|
|---|---|---|---|---|---|
|**GBIC**|Gigabit Interface Converter|1 Gbps|ألياف|~550 م|قديم وكبير الحجم، استُبدل بـ SFP|
|**SFP**|Small Form-factor Pluggable|1 Gbps|ألياف / نحاس|حتى 10 كم|الأكثر استخدامًا في شبكات Gigabit|
|**SFP+**|—|10 Gbps|ألياف|حتى 10 كم|نفس حجم SFP لكن أسرع|
|**QSFP / QSFP+ / QSFP28**|Quad SFP Form|40–100 Gbps|ألياف|حتى 40 كم|يُستخدم في مراكز البيانات|
|**BiDi (Bidirectional)**|—|1–10 Gbps|ألياف مفردة|حتى 10 كم|يرسل ويستقبل على نفس الليف بموجتين مختلفتين|
|**RJ-45 Copper SFP**|—|1 Gbps|كابلات Ethernet (Cat 5e/6)|حتى 100 م|لتحويل المنفذ من Fiber إلى Copper|

---

### 🌈 **الأطوال الموجية (Wavelengths)**

|الطول الموجي|نوع الألياف|الاستخدام|المدى التقريبي|
|---|---|---|---|
|**850 nm**|Multimode Fiber (MMF)|مسافات قصيرة|~300–400 م|
|**1310 nm**|Singlemode Fiber (SMF)|مسافات متوسطة|~10 كم|
|**1550 nm**|Singlemode Fiber (SMF)|مسافات طويلة جدًا|~40 كم +|

---

### 🧠 **خصائص إضافية مهمة**

- **Hot-swappable:** يمكن تبديله أثناء تشغيل الجهاز.
    
- **DDM (Digital Diagnostic Monitoring):** مراقبة الحرارة، الجهد، والطاقة الضوئية.
    
- **Loopback Test:** لاختبار سلامة المنفذ أو الكابل.
    
- **Compatibility:** لا تخلط بين MMF و SMF أو تستخدم موصلات غير مطابقة.
    

---

### ⚖️ **مقارنة سريعة**

|النوع|السرعة|المدى|الوسيط|قابل للتبديل|
|---|---|---|---|---|
|**SFP**|1 Gbps|حتى 10 كم|Fiber / Copper|✅|
|**SFP+**|10 Gbps|حتى 10 كم|Fiber|✅|
|**QSFP**|40–100 Gbps|حتى 40 كم|Fiber|✅|
|**RJ-45 SFP**|1 Gbps|حتى 100 م|Copper|✅|

---

### 📌 **الخلاصة للامتحان**

- **SFP ↔ 1 Gbps** — الأكثر شيوعًا.
    
- **SFP+ ↔ 10 Gbps** — نفس الشكل لكن أسرع.
    
- **QSFP ↔ 40–100 Gbps** — لمراكز البيانات.
    
- **850 nm = MMF / Short range**، **1310 nm = SMF / Medium**، **1550 nm = SMF / Long range**.
    
- **Hot-swappable + DDM** = من خصائص SFP الحديثة.
---

## 🌍 **Network Types & Architectures – CompTIA Network+ (Objective 1.6)**

---

### 🔹 **أولًا: أنواع البنى الأساسية (Network Types)**

|النوع|الاسم|الوصف|
|---|---|---|
|**LAN**|Local Area Network|شبكة محلية في موقع واحد مثل مكتب أو مبنى، بسرعات تصل إلى 1–10 Gbps.|
|**WLAN**|Wireless LAN|شبكة محلية لاسلكية تعتمد على Wi-Fi.|
|**WAN**|Wide Area Network|تربط مواقع بعيدة عبر الإنترنت أو خطوط مؤجرة (Leased Lines).|
|**MAN**|Metropolitan Area Network|تغطي مدينة أو نطاقًا حضريًا، مثل شبكات الجامعات أو المدن الذكية.|
|**PAN**|Personal Area Network|تربط أجهزة شخصية قريبة (Bluetooth, NFC).|
|**CAN**|Campus Area Network|تربط عدة مبانٍ ضمن موقع واحد (جامعة أو مجمع شركات).|
|**SAN**|Storage Area Network|شبكة مخصصة لنقل بيانات التخزين بين الخوادم وأجهزة التخزين.|

---

### 🔹 **ثانيًا: النماذج المعمارية (Architectural Models)**

#### 🧩 **1. Client–Server Architecture (العميل والخادم)**

- **الخادم** يقدم الخدمة (ملفات، طباعة، ويب...).
    
- **العميل** يطلبها ويستهلكها.
    
- **المميزات:** تحكم مركزي وأمان أعلى.
    
- **العيوب:** إذا تعطل الخادم تتوقف الخدمة.
    
- **أمثلة:** خوادم البريد، خوادم الملفات، خوادم الويب.
    

#### 🧩 **2. Peer-to-Peer (نظير إلى نظير)**

- كل جهاز يمكن أن يكون خادمًا وعميلًا في الوقت نفسه.
    
- تُستخدم في البيئات الصغيرة ومشاركة الملفات.
    
- **العيوب:** أمان ضعيف وصعوبة الإدارة.
    
- **أمثلة:** Windows Workgroup، BitTorrent.
    

#### 🧩 **3. Three-Tier Architecture (ثلاث الطبقات)**

|الطبقة|الوظيفة|الأمثلة|
|---|---|---|
|**Access Layer**|اتصال المستخدمين والأجهزة النهائية (PCs, Printers).|VLAN Access|
|**Distribution Layer**|توصيل Access بـ Core، وتنفيذ سياسات VLAN وRouting.|L3 Switches|
|**Core Layer**|العمود الفقري للشبكة، يربط كل شيء بسرعة عالية.|Backbone Routers|

🟢 **المميزات:** أداء عالي وتنظيم واضح للشبكات المتوسطة والكبيرة.

#### 🧩 **4. Spine–Leaf Architecture (العمود والأوراق)**

- تصميم حديث لمراكز البيانات.
    
- **Spine Switches** = النواة الأساسية.
    
- **Leaf Switches** = تتصل بالأجهزة والخوادم.
    
- كل Leaf يتصل بكل Spine مباشرة لتقليل التأخير.
    
- **ميزة:** لا عنق زجاجة (No Bottleneck) وسهل التوسع الأفقي.
    

---

### 🔹 **ثالثًا: البنى الافتراضية والحديثة (Modern & Virtualized Architectures)**

#### ⚙️ **1. Software-Defined Networking (SDN)**

- تفصل بين:
    
    - **Control Plane** (العقل/التحكم)
        
    - **Data Plane** (التنفيذ)
        
- الإدارة تتم عبر **Controller مركزي** يبرمج السويتشات.
    
- **الفائدة:** مرونة في التحكم وسهولة التوسع في مراكز البيانات.
    

#### ☁️ **2. Cloud-Based Networks**

- استخدام موارد سحابية بدل أجهزة محلية.
    
- **الأنواع:**
    
    - Public Cloud → مثل AWS, Azure
        
    - Private Cloud → داخل المؤسسة
        
    - Hybrid Cloud → مزيج بين الاثنين
        
- **الفائدة:** خفض التكاليف وسهولة الإدارة.
    

#### 🧱 **3. Zero Trust Architecture (ZTA)**

- لا يتم الوثوق بأي مستخدم أو جهاز افتراضيًا — حتى داخل الشبكة.
    
- يعتمد على **التحقق المستمر (Continuous Verification)** و**مبدأ أقل صلاحية (Least Privilege)**.
    
- **الهدف:** تقليل المخاطر الداخلية في الشبكات الكبيرة والموزعة.
    

#### ⚡ **4. Edge Computing**

- نقل المعالجة من السحابة إلى **حافة الشبكة (Edge)** قرب المستخدم.
    
- **الفائدة:** تقليل التأخير (Latency) وزيادة الكفاءة.
    
- **أمثلة:** أجهزة IoT، الكاميرات الذكية، السيارات المتصلة.
    

---

### 🔹 **رابعًا: البنى اللاسلكية (Wireless Architectures)**

|النوع|الوصف|الاستخدام|
|---|---|---|
|**Standalone APs**|نقاط وصول مستقلة يتم إعدادها يدويًا.|الشبكات الصغيرة.|
|**Controller-based APs**|نقاط وصول تدار مركزيًا من Wireless Controller.|المؤسسات الكبرى.|
|**Mesh Network**|كل AP يتصل بالآخر لتغطية أوسع.|المدن الذكية والمزارع.|

---

### 🔹 **خامسًا: الشبكات المتكاملة (Converged Networks)**

- شبكة واحدة تنقل **الصوت، الفيديو، والبيانات**.
    
- تعتمد على **QoS (Quality of Service)** لتحديد أولويات المرور.
    
- **أمثلة:** VoIP، مكالمات Teams/Zoom، بث الفيديو عبر نفس البنية.
    

---

### 🧠 **نصائح الاختبار (Network+ Exam Tips)**

1. اربط كل نوع شبكة بنطاقه:
    
    - **LAN → مبنى**
        
    - **CAN → جامعة أو مجمع**
        
    - **MAN → مدينة**
        
    - **WAN → دولي**
        
2. احفظ تسلسل **Three-Tier Architecture**  
    (Access → Distribution → Core).
    
3. تذكّر أن **Spine–Leaf** تصميم خاص بـ **Data Centers**.
    
4. **SDN** = تحكم مركزي قابل للبرمجة.  
    **Zero Trust** = لا ثقة بدون تحقق.
    
5. **Edge Computing** = المعالجة أقرب للمستخدم لتقليل الـLatency.
---
## **Software-Defined Networking (SDN) — CompTIA Network+ (Objective 1.6)**

---

### 🔹 **الفكرة الأساسية**

**SDN = Software-Defined Networking**  
تعني فصل **التحكم في الشبكة (Control Plane)** عن **تمرير البيانات (Data Plane)**.  
بدل أن يتخذ السويتش أو الراوتر القرارات ويُنفّذها محليًا، تُدار كل السياسات مركزيًا عبر **SDN Controller** ذكي يتحكم بجميع الأجهزة برمجيًا.

---

### ⚙️ **بنية SDN (Architecture)**

|الطبقة|الاسم|الدور|
|---|---|---|
|**1️⃣ Application Layer**|تطبيقات الإدارة والسياسات|تحتوي على تطبيقات الأمان، المراقبة، والأتمتة (Automation Apps).|
|**2️⃣ Control Layer**|**SDN Controller**|العقل المركزي الذي يترجم السياسات إلى أوامر.|
|**3️⃣ Data Layer**|أجهزة الشبكة (Switches / Routers)|تنفّذ الأوامر فعليًا بتمرير الترافيك حسب تعليمات Controller.|

---

### 🧩 **كيف يعمل SDN فعليًا**

1. **التطبيقات (Applications)** تطلب سياسات محددة، مثل:
    
    > "احظر هذا البروتوكول عن شبكة X."
    
2. **الـ Controller** يترجم القرار إلى أوامر تقنية باستخدام بروتوكولات مثل:
    
    - **OpenFlow**
        
    - **NETCONF**
        
    - **REST APIs**
        
3. **الأجهزة (Data Plane)** تنفّذ مباشرة دون الحاجة لمعرفة “السبب”، فقط “كيف تنفذ”.
    

---

### 📡 **أنواع Planes في SDN**

|الـ Plane|الوظيفة|
|---|---|
|**Data Plane**|تمرير الحِزَم (Packets) فعليًا – يعمل داخل Switches و Routers.|
|**Control Plane**|اتخاذ قرارات التوجيه وإدارة الجداول (Routing Tables).|
|**Management Plane**|مراقبة الشبكة وتعديل الإعدادات (CLI / SNMP / APIs).|

🔸 في SDN يتم **فصل Control عن Data Plane** لتصبح الإدارة **مركزية، ذكية، قابلة للبرمجة**.

---

### 💡 **المزايا الرئيسة**

1. **مرونة (Flexibility):** تعديل السياسات من واجهة مركزية بدل الدخول لكل جهاز.
    
2. **أتمتة (Automation):** التغييرات تتم آليًا عبر سكربتات أو Orchestrators.
    
3. **رؤية شاملة (Visibility):** Controller يرى كامل التوبولوجي ويتحكم بالمسارات لحظيًا.
    
4. **قابلية التوسع (Scalability):** مثالي لمراكز البيانات والـ Cloud Networks.
    

---

### ⚠️ **التحديات**

- الاعتماد العالي على الـ Controller (قد يصبح Single Point of Failure إن لم يُنسخ).
    
- الحاجة إلى مهارات برمجية (Python / REST API).
    
- صعوبة التكامل مع الأنظمة القديمة (Legacy Integration).
    

---

### 🌍 **مثال واقعي**

في شبكة تقليدية:

> إذا حدث ازدحام على Switch معيّن، يجب تعديل VLANs أو Routes يدويًا.

في SDN:

> الـ Controller يكتشف الازدحام ويعيد توزيع الترافيك تلقائيًا خلال ثوانٍ.

---

### 🧩 **تذكّر في الامتحان**

|السؤال|الجواب المختصر|
|---|---|
|ما الذي يميز SDN عن الشبكات التقليدية؟|**فصل Control عن Data Plane** وإدارة مركزية عبر Software.|
|ما دور Controller؟|اتخاذ قرارات التوجيه وإرسالها للأجهزة.|
|ما البروتوكول الشائع للتواصل بين Controller والأجهزة؟|**OpenFlow**|
|ما فائدة SDN؟|الأتمتة، المرونة، والتحكم البرمجي المركزي.|



---
---


## 🧠 **VXLAN – Virtual Extensible LAN(1.8)**

---

### 🏗️ الفكرة العامة

**VXLAN** = _Virtual eXtensible Local Area Network_  
تم ابتكاره لحل مشكلة أن **الشبكات المحلية (VLANs)** في مراكز البيانات **وصلت حدّها** — حيث لا يمكن أن تتجاوز 4096 شبكة (بسبب حدّ 12-bit VLAN ID).

VXLAN جاء ليقول:

> “لن نربط الشبكات بالأسلاك فقط، بل سنُمدّها افتراضيًا عبر الإنترنت أو عبر شبكات أخرى.”

بمعنى آخر:  
**VXLAN يسمح بتمديد VLAN عبر شبكات IP كبيرة (Layer 3).**

---

## ⚙️ **كيف يعمل VXLAN**

### 1️⃣ الفكرة الأساسية – _Encapsulation_

VXLAN يُغلِّف إطارات Layer 2 داخل **حزم UDP** (Layer 4)،  
ثم يُرسلها عبر شبكة IP (Layer 3).

يشبه هذا ما يفعله **GRE** أو **IPsec Tunnel**، لكنه مخصص للـ **Ethernet frames**.

---

### 2️⃣ **المكوّن الأساسي – VTEP**

|المصطلح|المعنى|
|---|---|
|**VTEP – VXLAN Tunnel Endpoint**|هو الجهاز (عادة switch أو hypervisor) الذي يقوم بعملية **Encapsulation** و**Decapsulation**.|

- عندما تخرج Frame من VLAN 10 مثلاً، الـ VTEP يُغلّفها داخل حزمة UDP.
    
- تُسافر الحزمة عبر شبكة IP.
    
- VTEP في الطرف الآخر **يفك التغليف** ويُعيدها إلى VLAN 10 كما كانت.
    

---

### 3️⃣ **VXLAN Network Identifier (VNI)**

بدل VLAN ID المكوّن من 12 bit،  
VXLAN يستخدم **24 bit VNI** → يعطيك أكثر من **16 مليون شبكة افتراضية**.

|العنصر|VLAN|VXLAN|
|---|---|---|
|المعرّف|12-bit|24-bit|
|العدد الأقصى للشبكات|4096|16,777,216|
|النطاق|Layer 2|Layer 3 Overlay|

---

## 🌐 **الشبكة المادية مقابل الافتراضية**

|النوع|الوصف|
|---|---|
|**Underlay**|الشبكة الفعلية – الكابلات، الراوترات، الـ IP الحقيقي.|
|**Overlay**|الشبكة الافتراضية – حيث تعمل VXLAN، تُنشأ فوق الـ Underlay.|

الـ VXLAN يخلق **Overlay Network** فوق بنية IP عادية.

---

## 💡 **فوائد VXLAN**

1. ✅ **توسّع هائل** – من 4096 VLAN إلى 16 مليون VNI.
    
2. 🔄 **عزل مرن** – كل مستأجر في مركز البيانات لديه شبكة Layer 2 خاصة به حتى عبر نطاق WAN.
    
3. ⚙️ **قابلية الأتمتة** – مهيّأ ليُدار عبر SDN Controllers.
    
4. 🌍 **استقلال عن Layer 2** – لم تعد الشبكة تحتاج امتدادًا ماديًا عبر Switches.
    

---

## ⚠️ **التحديات والملاحظات**

- يتطلب دعمًا من الأجهزة أو من الـ Hypervisors (مثل VMware NSX أو Cisco ACI).
    
- زيادة طفيفة في الحمل (Overhead) بسبب **Encapsulation Header** (حوالي 50 Byte زيادة).
    
- تحتاج إلى **MTU أكبر** (مثل 1600) لتفادي تجزئة الحزم.
    

---

## 🧩 **مثال عملي مبسّط**

> لديك مركز بيانات في الرياض وآخر في جدة.  
> كلاهما يستخدم VLAN 10.  
> تربطهما عبر VXLAN، فيتصرّفان كأنهما على نفس VLAN بالضبط — حتى لو كانت المسافة بينهما مئات الكيلومترات.

---

## 📘 **في الامتحان، تذكّر:**

|السؤال|الجواب المختصر|
|---|---|
|ما الغرض من VXLAN؟|توسيع VLAN عبر Layer 3 شبكات IP.|
|ما دور VTEP؟|تنفيذ Encapsulation/Decapsulation لإطارات VXLAN.|
|ما البروتوكول المستخدم في VXLAN؟|**UDP (port 4789)**|
|كم bit في VNI؟|**24 bit ≈ 16 مليون شبكة.**|
|ما الفرق بين Underlay و Overlay؟|Underlay = الشبكة الحقيقية، Overlay = الافتراضية.|

---
### DCI 
## 🏢 أولًا: ما هو **DCI (Data Center Interconnect)**؟

هو ببساطة:

> **ربط مركزين أو أكثر من مراكز البيانات (Data Centers) بحيث تعمل وكأنها شبكة واحدة.**

تُستخدم فيه تقنيات متقدمة لتمديد **الشبكات المحلية (VLANs)** و**الخدمات الافتراضية (VMs)** بين مراكز البيانات المتباعدة جغرافيًا — مثلاً بين **الرياض وجدة**.

---

## ⚙️ ثانيًا: ما علاقة **VXLAN** بالـ **DCI**

من قبل، كان ربط مراكز البيانات يعتمد على تقنيات Layer 2 حقيقية مثل:
‎ثانيًا: ما علاقة VXLAN بـ DCI

- **MPLS L2VPN**
    
- **VPLS**
    
- **OTV (Overlay Transport Virtualization – من Cisco)**
    

لكنها محدودة وصعبة التوسع.  
جاءت **VXLAN + SDN** لتكون الحل العصري، لأنها:

- تمدّ شبكات Layer 2 عبر Layer 3 بسهولة.
    
- تتيح إدارة مركزية عبر SDN Controller.
    
- تعمل فوق أي بنية تحتية IP (Underlay).
    

🎯 لذلك اليوم، أكثر تصميمات DCI الحديثة تستخدم:

> **VXLAN + EVPN (Ethernet VPN)**  
> كحل رسمي ومعتمد لتطبيق DCI.

---

## 🧩 ثالثًا: مكوّنات DCI الحديثة

|المكوّن|الوظيفة|
|---|---|
|**VTEP**|يمثل نقطة الدخول/الخروج لكل Data Center.|
|**VXLAN**|ينشئ النفق (Tunnel) بين المراكز لنقل إطارات L2 داخل حزم IP.|
|**EVPN**|بروتوكول تحكم (Control Plane) لإدارة الجداول بين المراكز.|
|**SDN Controller / BGP-EVPN**|يدير ويُنسّق الاتصال والسياسات بين المواقع.|

---

## 🌍 رابعًا: سيناريو عملي

> لديك مركز بيانات في **الرياض** يحتوي على VLAN 10 لأجهزة العملاء،  
> ومركز بيانات في **جدة** يحتوي على نفس VLAN 10.

بدل تمديد كابل أو MPLS L2VPN، تستخدم:

- **في اكس لان VXLAN**: لتمديد VLAN عبر شبكة IP (الإنترنت أو WAN).
    
- **إي في بي إن EVPN**: لمزامنة جداول الـ MAC وARP بين المراكز.
    

النتيجة:  
كلا المركزين يتصرفان كأنهما **شبكة LAN واحدة ممتدة** رغم أنهما في مدينتين مختلفتين.

---

## 🔒 خامسًا: مزايا DCI الحديثة (VXLAN/EVPN)

1. **مرونة هائلة** – نقل VMs أو الحاويات (Containers) بين المراكز بسهولة.
    
2. **أمان أعلى** – باستخدام Segmentation عبر VNI.
    
3. **تحكم ذكي** – بفضل الـ SDN Controllers.
    
4. **لا تحتاج MPLS** – تعمل فوق أي IP Network.
    
5. **قابلية توسّع كبيرة** – تدعم مئات المراكز دون تعقيد.
    

---

## 🧠 باختصار:

| المفهوم   | الدور                        |
| --------- | ---------------------------- |
| **VLAN**  | داخل مركز بيانات واحد        |
| **VXLAN** | تمديد VLAN عبر Layer 3       |
| **DCI**   | ربط مراكز بيانات متعددة      |
| **EVPN**  | نظام تحكم ذكي داخل VXLAN DCI |
| **SDN**   | إدارة مركزية لسياسات الشبكة  |


---


# 🧠 **Zero Trust Architecture (ZTA)1.8**

---

## ⚙️ الفكرة الجوهرية

**زيرو تروست Zero Trust** تعني بالبساطة:

> لا تثق بأحد… حتى لو كان داخل شبكتك.

في الماضي، كان النموذج الأمني الكلاسيكي يقول:

> “من يدخل الشبكة الداخلية، فهو موثوق.”  
> لكن اليوم، بعد انتشار العمل عن بُعد، والسيرفرات السحابية، وتعدد الأجهزة، صار هذا المفهوم خطيرًا جدًا.

📌 لذلك جاءت **Zero Trust** لتقول:

> "الثقة لا تُمنح بالافتراض، بل تُكتسب في كل طلب وصول (access request)."

---

## 🧩 الأساس الفلسفي لـ Zero Trust

|مبدأ|الشرح|
|---|---|
|**Never Trust, Always Verify**|لا تفترض الثقة أبدًا، تحقق من كل شيء وكل مرة.|
|**Least Privilege Access**|كل مستخدم أو نظام يحصل فقط على ما يحتاجه، لا أكثر.|
|**Assume Breach**|تصرّف وكأن الشبكة مُخترقة بالفعل، ووزّع الأمان على الطبقات.|

---

## 🧱 مكونات Zero Trust الرئيسية

1. **Identity Verification (التحقق من الهوية)**
    
    - كل طلب وصول يجب أن يمر بمصادقة قوية (مثل MFA).
        
    - تُستخدم تقنيات مثل **SSO**, **OAuth**, **Kerberos**, **FIDO2**.
        
2. **Device Trust (موثوقية الجهاز)**
    
    - النظام يتحقق من الجهاز نفسه: هل هو محدث؟ هل عليه برامج ضارة؟
        
    - إذا فشل الفحص → يُمنع الوصول حتى لو كان المستخدم موثوقًا.
        
3. **Network Segmentation (تقسيم الشبكة)**
    
    - لا توجد شبكة داخلية "آمنة بالكامل".
        
    - تُقسم الشبكة إلى مناطق (Zones) مثل:
        
        - User Zone
            
        - Server Zone
            
        - Database Zone
            
    - ويُستخدم **microsegmentation** لفصل الأنظمة بدقة.
        
4. **Continuous Monitoring (المراقبة المستمرة)**
    
    - كل نشاط يُراقب ويُسجّل.
        
    - تُستخدم أدوات SIEM, SOAR, AI Analytics لاكتشاف السلوك غير المعتاد.
        
5. **Encryption Everywhere (التشفير في كل الطبقات)**
    
    - من التصفح (HTTPS, TLS 1.3)
        
    - إلى البيانات المخزنة (at rest)
        
    - وحتى التبادل بين الأنظمة الداخلية.
        

---

## 🔐 مقارنة مع النموذج القديم

|الجانب|النموذج القديم|Zero Trust|
|---|---|---|
|الثقة|داخل الشبكة موثوق|لا ثقة مطلقة|
|الدخول|بناءً على الموقع|بناءً على الهوية والسياق|
|التحقق|لمرة واحدة|مستمر في كل جلسة|
|الوصول|كامل بعد المصادقة|محدود حسب الدور والسياسة|
|الأمان|محيط خارجي فقط (firewall)|مدمج في كل طبقة (endpoints, apps, users)|

---

## 🧠 مثال واقعي

> موظف يدخل إلى لوحة الإدارة من منزله.  
> النظام يتحقق من:
> 
> 1. من هو؟ (الهوية)
>     
> 2. من أين؟ (الموقع الجغرافي)
>     
> 3. بأي جهاز؟ (نظام التشغيل، مستوى الأمان)
>     
> 4. ماذا يريد أن يفعل؟ (الصلاحيات المطلوبة)
>     
> 
> إذا اجتاز كل ذلك، يحصل على وصول **مؤقت ومحدود** فقط، لا دائم.

---

## 🏗️ كيف تُنفّذ عمليًا في الشبكات

1. **استخدام NAC (Network Access Control)** للتحقق من الأجهزة عند الاتصال.
    
2. **استخدام SDN أو Firewalls ذكية** لتطبيق السياسات الدقيقة (microsegmentation).
    
3. **استخدام SIEM / SOAR** لتحليل السلوك ومراقبة الأنشطة.
    
4. **استخدام Identity Providers** مثل Azure AD, Okta, Google Identity.
    
5. **تطبيق سياسة Least Privilege** على جميع المستخدمين والحسابات.
    

---

## 💡 تذكّر في الامتحان

|سؤال محتمل|الإجابة|
|---|---|
|ما مبدأ Zero Trust؟|عدم الثقة بأي كيان بدون تحقق مستمر.|
|ما التقنية الأساسية لتحقيقه؟|المصادقة القوية + التقسيم + المراقبة.|
|هل يحمي من الهجمات الداخلية؟|نعم، لأنه لا يثق حتى بالمستخدمين الداخليين.|
|هل يعتمد على الجدران النارية فقط؟|لا، بل يوزع الأمان على كل الطبقات.|

---

## 🧩 المفهوم في جملة واحدة:

> 🔹 عملياً: Zero Trust = “تحقق دائم + وصول محدود + مراقبة مستمرة.”  
> 🔹 الهدف: حماية الهوية، الجهاز، والبيانات في بيئة لم تعد فيها الحدود الشبكية واضحة.


---


## 🏗️ **Infrastructure as Code (IaC)1.8**

مفهوم حديث يربط بين **الشبكات** و**البرمجة** و**الأتمتة**، ويُعد أحد أهم مفاتيح التحول من **“إدارة الشبكات يدويًا”** إلى **“إدارة الشبكات ككود”**.

---

## 🧠 أولاً: ما هو مفهوم Infrastructure as Code؟

**Infrastructure as Code** تعني:

> “إدارة البنية التحتية (الشبكات، الخوادم، التخزين، الجدران النارية...) باستخدام ملفات برمجية (كود)، بدل إعدادها يدويًا.”

<font color="#ff0000">بعبارة أخرى:</font>

- **بدل ما تفتح راوتر أو سويتش وتكتب أوامر CLI واحدة واحدة،**
    
- **تكتب كود أو سكربت يُنفّذ كل شيء أوتوماتيكيًا في ثوانٍ.**
    

---

## ⚙️ **فكرة IaC الأساسية**

IaC = **الأتمتة(Automation) + القابلية للتكرار + التوحيد**

|العنصر|المعنى|
|---|---|
|**Automation**|كل شيء يتم تلقائيًا بدون تدخل يدوي|
|**Consistency**|كل الأجهزة تُضبط بنفس الإعداد تمامًا|
|**Version Control**|يمكنك حفظ ومراجعة التغييرات كأنها كود في Git|
|**Scalability**|تنشئ مئات الخوادم أو الشبكات الجديدة بنفس النمط بسهولة|

---

## 🧩 **المقارنة بين الطريقة القديمة والجديدة**

|الجانب|الطريقة التقليدية|Infrastructure as Code|
|---|---|---|
|الإعداد|يدوي (CLI أو GUI)|عبر سكربت أو ملفات YAML|
|الخطأ البشري|مرتفع|منخفض جدًا|
|الوقت|بطيء|سريع جدًا|
|التكرار|صعب|سهل (نسخ الكود)|
|التوثيق|محدود|الكود نفسه هو التوثيق|
|التتبع (Versioning)|لا يوجد|باستخدام Git/GitHub|

---

## 🧰 **أشهر أدوات Infrastructure as Code**

|الأداة|الاستخدام الأساسي|ملاحظات|
|---|---|---|
|**Terraform**|إنشاء وإدارة البنية التحتية السحابية (AWS, Azure, GCP)|لغة HCL (HashiCorp Language)|
|**Ansible**|أتمتة الإعدادات على الخوادم وأجهزة الشبكة|يستخدم ملفات YAML، لا يتطلب Agent|
|**Puppet**|إدارة الإعدادات بشكل مستمر|جيد للأنظمة الكبيرة|
|**Chef**|إدارة إعدادات الخوادم ككود|يعتمد على لغة Ruby|
|**CloudFormation (AWS)**|IaC خاص بـ AWS|مدمج في منصة أمازون|
|**SaltStack**|إدارة وأتمتة الأنظمة الكبيرة|مفتوح المصدر|

---

## 🧱 **أنواع IaC (طرائق التنفيذ)**

|النوع|الوصف|مثال|
|---|---|---|
|**Declarative (تصريحي)**|تقول _ماذا تريد_ وليس _كيف تنفّذه_|Terraform, Ansible|
|**Imperative (أمري)**|تكتب خطوات التنفيذ واحدة واحدة|Python Script, Bash|

> 🔸 _Declarative_ أكثر شيوعًا لأنها تتيح للكود نفسه أن يتحقق من الحالة الفعلية ويصححها تلقائيًا.

---

## 🌐 **كيف يربط IaC الشبكات بالبنية السحابية؟**

IaC يمكّنك من:

- إنشاء **VPCs، Subnets، Security Groups** في AWS مثلًا عبر كود.
    
- نشر **Routers, Switches, Firewalls** افتراضية في بيئة سحابية.
    
- إدارة إعدادات الشبكات بنفس طريقة إدارة البرامج.
    


---

## 🧪 **مفاهيم مرتبطة بالـ IaC**

|المصطلح|الشرح|
|---|---|
|**Immutable Infrastructure**|بدلاً من تعديل الأجهزة، يُعاد نشرها بالكامل كنسخة جديدة من الكود.|
|**Configuration Drift**|الاختلافات التي تظهر بمرور الوقت بين الأجهزة — IaC يمنعها.|
|**GitOps**|ربط IaC مع Git لتطبيق التغييرات بمجرد تعديل الكود.|
|**CI/CD**|دمج IaC مع خطوط النشر الآلي (Continuous Integration / Delivery).|


---

## 💡 **تشبيه عملي**

تخيل أن لديك **مطبخ مطعم**:

- الطريقة القديمة: كل طباخ يطبخ بطريقته (فوضى).
    
- IaC: لديك **وصفة مكتوبة بدقة**، كل طباخ ينفذها خطوة بخطوة — نفس النتيجة دائمًا.
    

---

## 📖 **خلاصة الدرس**

|المفهوم|التوضيح|
|---|---|
|Infrastructure as Code|إدارة البنية التحتية عن طريق كود|
|الهدف|أتمتة، سرعة، توحيد، تتبع|
|الأدوات|Terraform, Ansible, Puppet, Chef|
|الفائدة للشبكات|إعداد الشبكات سحابيًا أو محليًا بكود موحّد|
|العلاقة بـ DevOps|IaC هو قلب مبدأ DevOps|


---

## 🔗 **العلاقة بين Playbooks و IaC**

- **IaC**: يهتم ببناء وتشغيل البنية التحتية **(شبكات، خوادم، أنظمة)** عن طريق الكود.
    
- **Playbooks (في الأمن)**: تهتم بأتمتة **الاستجابة للحوادث الأمنية**.
    

لكن كلاهما يعتمد على نفس **الفلسفة:**

> “التعامل مع العمليات التقنية على أنها كود يمكن تشغيله، مراجعته، وإعادة استخدامه.”


---

---

## 🧩 **Playbooks — ما هي؟**

**Playbook** هي خطة جاهزة ومنظمة من **خطوات محددة مسبقًا** تُستخدم عند وقوع حادث أمني أو مهمة معينة.

### 🔹 تعريفها:

> مجموعة من **الإجراءات الشرطية** (Conditional Steps) تُنفّذ بناءً على نوع الحدث الأمني.

---

## ⚙️ **ما تحتوي عليه Playbook:**

|العنصر|الشرح|
|---|---|
|**Conditional Steps**|خطوات تعتمد على نوع الحادث (مثلاً: هل هو Data Breach؟ هل هو Ransomware؟)|
|**Step-by-Step Procedures**|خطوات متسلسلة قابلة لإعادة الاستخدام — مثل قالب جاهز Template|
|**Reusable Template**|يمكن استخدامها مرارًا في حوادث متشابهة|
|**Automation Integration**|يمكن ربطها بأدوات أتمتة لتعمل تلقائيًا|

---

## 🤖 **الدمج مع SOAR Platforms**

- **SOAR = Security Orchestration, Automation, and Response**  
    أي: منصة تجمع بين التنسيق، الأتمتة، والاستجابة.
    

### 🔸 التكامل:

Playbooks عادة تُستخدم داخل أنظمة SOAR لتقوم بـ:

- جمع بيانات من أدوات مختلفة (firewall, SIEM, IDS...)
    
- اتخاذ قرارات آلية (مثل عزل جهاز، إيقاف مستخدم)
    
- تنفيذ أوامر استجابة فورية عند الحوادث الأمنية.
    

---

## 🔒 **أمثلة واقعية على Playbooks:**

|الحالة|الإجراءات داخل الـ Playbook|
|---|---|
|**Ransomware Attack**|عزل النظام المصاب → تنبيه الفريق → استعادة النسخة الاحتياطية|
|**Data Breach Investigation**|تحديد المستخدمين المتأثرين → استخراج السجلات → تنبيه الـ SOC|
|**Phishing Email**|فحص المرسل → تحليل الرابط → حذف البريد المشبوه من جميع صناديق البريد|

---


## 📘 **CompTIA Network+ – Common Ports, Protocols, and Services**

|**Protocol / Service**|**Port (TCP/UDP)**|**Description / Use Case**|
|---|---|---|
|**FTP** (File Transfer Protocol)|20, 21|نقل الملفات بين الأنظمة (غير مشفر)|
|**SFTP** (Secure File Transfer Protocol)|22|نقل الملفات بأمان عبر SSH|
|**SSH** (Secure Shell)|22|اتصال آمن لإدارة الأنظمة عن بُعد|
|**Telnet**|23|اتصال نصي غير مشفر (قديم، غير آمن)|
|**SMTP** (Simple Mail Transfer Protocol)|25|إرسال البريد الإلكتروني|
|**DNS** (Domain Name System)|53|تحويل أسماء النطاق إلى عناوين IP|
|**DHCP** (Dynamic Host Configuration Protocol)|67, 68|توزيع عناوين IP تلقائيًا للأجهزة|
|**TFTP** (Trivial File Transfer Protocol)|69|نقل ملفات بسيط بدون مصادقة|
|**HTTP** (Hypertext Transfer Protocol)|80|نقل صفحات الويب (غير مشفر)|
|**NTP** (Network Time Protocol)|123|مزامنة الوقت بين الأنظمة|
|**SNMP** (Simple Network Management Protocol)|161, 162|مراقبة وإدارة الأجهزة في الشبكة|
|**LDAP** (Lightweight Directory Access Protocol)|389|الوصول إلى خدمات الدليل (مثل Active Directory)|
|**HTTPS** (Hypertext Transfer Protocol Secure)|443|تصفح الويب الآمن باستخدام SSL/TLS|
|**SMB** (Server Message Block)|445|مشاركة الملفات والطابعات في ويندوز|
|**Syslog**|514|إرسال سجلات النظام إلى خوادم مركزية|
|**SMTPS** (Secure SMTP)|587|إرسال البريد الإلكتروني عبر SSL/TLS|
|**LDAPS** (LDAP over SSL)|636|اتصال آمن بخدمات الدليل|
|**SQL Server**|1433|اتصال بخوادم Microsoft SQL|
|**RDP** (Remote Desktop Protocol)|3389|اتصال سطح مكتب عن بُعد|
|**SIP** (Session Initiation Protocol)|5060, 5061|بدء جلسات الصوت والفيديو عبر الإنترنت (VoIP)|

---
## 📘 **1.5 – Transmission Media and Transceivers**

|**Category**|**Items (as listed in official objectives)**|
|---|---|
|**Wireless**|• 802.11 standards  <br>• Cellular  <br>• Satellite|
|**Wired**|• 802.3 standards  <br>• Single-mode vs. multimode fiber  <br>• Direct attach copper (DAC) cable  <br>  ○ Twinaxial cable  <br>• Coaxial cable  <br>• Cable speeds  <br>• Plenum vs. non-plenum cable|
|**Transceivers**|• Protocol  <br>  ○ Ethernet  <br>  ○ Fibre Channel (FC)  <br>• Form factors  <br>  ○ Small form-factor pluggable (SFP)  <br>  ○ Quad small form-factor pluggable (QSFP)|
|**Connector Types**|• Subscriber connector (SC)  <br>• Local connector (LC)  <br>• Straight tip (ST)  <br>• Multi-fiber push on (MPO)  <br>• Registered jack (RJ)11  <br>• RJ45  <br>• F-type  <br>• Bayonet Neill–Concelman (BNC)|
