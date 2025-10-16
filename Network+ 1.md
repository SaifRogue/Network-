### 📚 OSI Model – CompTIA Network+ (Objective 1.1)





---
### 🔹 الطبقات السبعة في نموذج OSI:


1. **Layer 1 – Physical (الطبقة الفيزيائية)**
    
    - مسؤولة عن الإشارات الكهربائية/الضوئية، الكابلات، الموصلات.
        
    - مثال: Ethernet cables، fiber optics.
        
2. **Layer 2 – Data Link (رابط البيانات)**
    
    - يتعامل مع **MAC addresses** وإطارات البيانات (frames).
        
    - مسؤول عن **error detection/correction** مثل CRC.
        
    - مثال: Switches.
        
3. **Layer 3 – Network (الشبكة)**
    
    - يحدد **IP addresses** ويختار أفضل مسار (routing).
        
    - مثال: Routers، بروتوكولات مثل OSPF, BGP.
        
4. **Layer 4 – Transport (النقل)**
    
    - يحدد **TCP vs UDP**.
        
    - مسؤول عن **segmentation, flow control, error recovery**.
        
5. **Layer 5 – Session (الجلسة)**
    
    - ينشئ ويدير جلسات الاتصال بين الأجهزة.
        
    - يتعامل مع **authentication, authorization, session management**.
        
6. **Layer 6 – Presentation (العرض)**
    
    - يحوّل البيانات إلى صيغة مفهومة: **encryption, compression, encoding**.
        
    - مثال: SSL/TLS، ASCII.
        
7. **Layer 7 – Application (التطبيق)**
    
    - أقرب للمستخدم النهائي.
        
    - بروتوكولات مثل HTTP, SMTP, DNS.
        

---


### الطبقات السبع (من الأعلى إلى الأسفل):

| الطبقة | الاسم        | الوظيفة                                             |
| ------ | ------------ | --------------------------------------------------- |
| 7️⃣    | Application  | التفاعل مع المستخدم (مثل المتصفح، البريد، FTP)      |
| 6️⃣    | Presentation | التشفير، الضغط، وتحويل البيانات إلى تنسيق مشترك     |
| 5️⃣    | Session      | إنشاء، إدارة، بدء وإنهاء الجلسات بين التطبيقات      |
| 4️⃣    | Transport    | نقل البيانات وضمان وصولها (TCP/UDP)                 |
| 3️⃣    | Network      | تحديد أفضل مسار للبيانات (IP, Routers)              |
| 2️⃣    | Data Link    | عنونة الأجهزة (MAC)، والتحكم بالوصول للوسيط         |
| 1️⃣    | Physical     | إرسال البتات عبر الكيبل أو الوسيط (الكهرباء، الضوء) |
- **Layer 5 – Session**
    
    - **وظائف**: Authentication (مصادقة)، Authorization (تفويض)، Session management (إدارة الجلسات).
        
- **Layer 4 – Transport**
    
    - **وظائف**: Segmentation (تجزئة البيانات)، Flow control (التحكم في التدفق)، TCP/UDP (اختيار البروتوكول).
        
- **Layer 3 – Network**
    
    - **وظائف**: IP addressing، Routing (اختيار أفضل مسار).
        
- **Layer 2 – Data Link**
    
    - **وظائف**: Framing (تجميع البتات في إطارات)، Error detection (كشف الأخطاء باستخدام CRC).
- **Layer 1 – Physical (الفزيائية)**
    

- **وظائف**: نقل الـ **Bits** كإشارات كهربائية/ضوئية/لاسلكية عبر الوسيط.
    
- أمثلة: الكابلات (UTP, Fiber), الموصلات (RJ45, SC), أجهزة بسيطة مثل Hubs, Repeaters.

---

### 📌 الفرق بين OSI و TCP/IP

- OSI = **7 طبقات** (مفهوم تعليمي).
    
- TCP/IP = **4 طبقات** (مستخدم عمليًا: Application, Transport, Internet, Network Access).

---
---
---


![[Pasted image 20251001013322.png]]
- **Layer 7 – Application**: `https://mail.google.com` (تطبيق فعلي يتفاعل مع المستخدم).
    
- **Layer 6 – Presentation**: **SSL encryption** (التشفير).
    
- **Layer 5 – Session**: يربط الـ Presentation مع الـ Transport (إدارة الجلسة).
    
- **Layer 4 – Transport**: **TCP encapsulation** (التغليف).
    
- **Layer 3 – Network**: **IP encapsulation** (إضافة عنوان IP).
    
- **Layer 2 – Data Link**: **Ethernet** (إطارات + MAC).
    
- **Layer 1 – Physical**: **Electrical signals** (إرسال البتات).


---
---
---


### 📘 **Networking Devices (Objective 1.2)**


---

## 🔹 أولًا: Networking Appliances (الأجهزة الفيزيائية والافتراضية)

- **Router (الراوتر)**
    
    - يربط الشبكات المختلفة (Layer 3).
        
    - يحدد أفضل مسار (Routing).
        
- **Switch (السويتش)**
    
    - يربط الأجهزة داخل نفس الشبكة المحلية (LAN).
        
    - Layer 2 (MAC) – يدعم أيضًا Layer 3 إذا كان Managed L3 switch.
        
- **Firewall (الجدار الناري)**
    
    - يفلتر الترافيك بين الشبكات (Traffic Filtering).
        
    - ممكن يكون Hardware أو Software.
        
- **IDS / IPS (Intrusion Detection / Prevention Systems)**
    
    - IDS = يكتشف الهجمات.
        
    - IPS = يكتشف ويمنع الهجمات.
        
- **Load Balancer**
    
    - يوزع الحمل (Traffic) على عدة خوادم لزيادة الكفاءة والتوافرية.
        
- **Proxy Server**
    
    - يعمل كوسيط بين المستخدم والإنترنت (Caching, Filtering).
        
- **NAS (Network-Attached Storage)**
    
    - تخزين مشترك عبر الشبكة.
        
- **SAN (Storage Area Network)**
    
    - شبكة متخصصة للتخزين عالي السرعة (عادة عبر Fiber).
        
- **Wireless Devices**
    
    - **Access Point (AP):** يربط الأجهزة اللاسلكية بالشبكة.
        
    - **Wireless Controller:** يدير عدة Access Points مركزياً.
        

---

## 🔹 ثانيًا: Applications

- **CDN (Content Delivery Network)**
    
    - شبكة موزعة لتسليم المحتوى بسرعة للمستخدمين عبر أقرب خادم.
        

---

## 🔹 ثالثًا: Functions

- **VPN (Virtual Private Network)**
    
    - اتصال آمن ومشفر عبر الإنترنت (tunnel).
        
- **QoS (Quality of Service)**
    
    - إدارة أولوية الترافيك (مثال: إعطاء أولوية لمكالمات VoIP).
        
- **TTL (Time To Live)**
    
    - حقل في IP packet يحدد عمر الحزمة ويمنع الحلقات اللانهائية.
        

---

### 🧾 ملخص سريع:

|الفئة|أمثلة|الوظيفة|
|---|---|---|
|**Appliances**|Router, Switch, Firewall, IDS/IPS, Load Balancer, Proxy, NAS, SAN, AP|توجيه، توزيع، حماية، تخزين|
|**Applications**|CDN|تسريع المحتوى|
|**Functions**|VPN, QoS, TTL|أمان، أولوية ترافيك، منع الحلقات|

---
---
---
### 📊 **Networking Devices vs OSI Layers**

|الجهاز|الطبقة الأساسية في OSI|ملاحظات إضافية|
|---|---|---|
|**Router**|**Layer 3 – Network**|مسؤول عن التوجيه (Routing) باستخدام IP addresses.|
|**Switch**|**Layer 2 – Data Link**|يعمل مع **MAC addresses**. (لو كان L3 Switch يقدر يشتغل في Layer 3 أيضًا).|
|**Firewall**|**Layer 3 – Network** (أساسي)  <br>**Layer 4 – Transport** (Ports)  <br>**Layer 7 – Application** (NGFW)|الفايروال التقليدي يفلتر IP/Port، بينما NGFW يقدر يفحص المحتوى (DPI).|
|**IDS/IPS**|**Layer 3/4 – Network & Transport**  <br>**Layer 7 – Application** (DPI)|IDS = يكشف الهجمات، IPS = يكشف + يمنع. غالبًا يراقب الباكيت عبر عدة طبقات.|
|**Access Point (AP)**|**Layer 2 – Data Link**|يربط الأجهزة اللاسلكية (Wi-Fi) بالشبكة المحلية.|
|**Load Balancer**|**Layer 4 – Transport** (TCP/UDP)  <br>**Layer 7 – Application** (HTTP/HTTPS)|يوزع الحمل على الخوادم. فيه نوع L4 & L7 Load Balancer.|

---

🔑 **الخلاصة للامتحان**:

- Router → L3
    
- Switch → L2 (أحيانًا L3)
    
- Firewall → L3 (أساسي) لكن ممكن يوصل L7 حسب النوع
    
- IDS/IPS → يشتغل على أكثر من طبقة (3,4,7)
    
- AP → L2
    
- Load Balancer → L4 أو L7

---
---
---




في **Network+ N10-009 – الهدف 1.2** مطلوب منك أن تفهم وتفرّق بين **Networking Functions** الرئيسية

---

## 🔹 Networking Functions (الوظائف الأساسية)

### 1. **VPN (Virtual Private Network)**

- ينشئ نفقًا (Tunnel) مشفرًا بين جهاز المستخدم والشبكة/الإنترنت.
    
- يحمي البيانات أثناء انتقالها عبر الشبكات العامة.
    
- يُستخدم للوصول الآمن إلى موارد داخلية أو للتصفح الآمن.
    

### 2. **QoS (Quality of Service)**

- إدارة أولوية مرور البيانات داخل الشبكة.
    
- أمثلة: إعطاء أولوية أعلى لمكالمات **VoIP** أو بث الفيديو على حساب تنزيل الملفات.
    
- يقلل من التأخير (Latency) والتقطيع (Jitter).
    

### 3. **TTL (Time To Live)**

- قيمة في رأس حزمة الـ IP.
    
- تحدد كم “قفزة” (hop) يمكن للحزمة أن تمر بها قبل أن تُسقط.
    
- تمنع الحلقات (loops) اللانهائية في الشبكات.
    

---

## 🧾 ملخص سريع

|الوظيفة|الهدف|مثال عملي|
|---|---|---|
|**VPN**|أمان وربط آمن|اتصال موظف عن بعد بخوادم الشركة|
|**QoS**|تحسين الأداء وإدارة الأولويات|أولوية لمكالمات Teams أو Zoom|
|**TTL**|منع الحلقات وضبط عمر الحزم|حزمة Ping تسقط بعد عدد قفزات محدد|


**CDN – Content Delivery Network** 👇

---

### 🔹 ما هو CDN؟

شبكة موزعة من **خوادم الكاش** (caching servers) موجودة في مواقع جغرافية مختلفة.

- بدل ما يطلب المستخدم البيانات من **الخادم الأصلي (Origin Server)** البعيد، يجيبها من **خادم قريب (Edge Server)**.
    
- هذا يقلل **الزمن المستغرق (Latency)** ويزيد سرعة تحميل المحتوى.
    

---

### 🔹 الفوائد

- **تسريع الوصول**: يقلل وقت تحميل الصفحات والفيديوهات.
    
- **التوزيع الجغرافي**: يضمن أن المستخدم في السعودية مثلًا يحصل على البيانات من خادم قريب (الرياض/دبي) بدل أمريكا.
    
- **تقليل الضغط على الخادم الأصلي**: لأنه يخدم نسخ مكررة Cached.
    
- **مخفي عن المستخدم النهائي**: المستخدم غالبًا لا يعرف أنه يتعامل مع CDN.
    

---

### 🔹 أمثلة عملية

- فيديوهات **YouTube**، صور **Instagram**، مواقع **Netflix** و **Facebook** كلها تستخدم CDNs.
    
- أشهر مزودي CDN: **Cloudflare, Akamai, Amazon CloudFront**.

---
---
---


### 🟦 مفاهيم وتقنيات السحابة:

- **NFV (Network Functions Virtualization):** تحويل وظائف الشبكة التقليدية (مثل الراوتر/الفايروال) إلى مكونات افتراضية تعمل على خوادم.
    
- **VPC (Virtual Private Cloud):** بيئة سحابية خاصة داخل سحابة عامة، تُمكّنك من عزل شبكتك.
    
- **Security Groups / Security Lists:** أدوات للتحكم بحركة المرور المسموح بها في بيئات السحابة (تشبه Access Control Lists).
    
- **Cloud Gateways:** مثل **Internet Gateway** و **NAT Gateway** لتسهيل الاتصال من/إلى السحابة.
    

### 🟦 خيارات الاتصال بالسحابة:

- **VPN:** ربط آمن مشفر بين شبكتك والسحابة.
    
- **Direct Connect:** خط مخصص مباشر للسحابة (أسرع وأكثر أمانًا من الإنترنت العام).
    

### 🟦 نماذج النشر (Deployment Models):

- **Public Cloud** → موارد سحابية مشتركة (AWS, Azure).
    
- **Private Cloud** → سحابة مخصصة لمؤسسة واحدة.
    
- **Hybrid Cloud** → مزيج من الاثنين مع إمكانية التكامل.
    

### 🟦 نماذج الخدمة (Service Models):

- **SaaS (Software as a Service):** مثل Gmail, Office 365 (تستخدم البرنامج مباشرة).
    
- **IaaS (Infrastructure as a Service):** مثل AWS EC2 (خوادم افتراضية).
    
- **PaaS (Platform as a Service):** مثل Google App Engine (بيئة تطوير جاهزة).
    

### 🟦 خصائص أساسية:

- **Scalability (قابلية التوسع):** زيادة الموارد عند الحاجة.
    
- **Elasticity (المرونة):** إضافة/إزالة الموارد تلقائيًا.
    
- **Multitenancy (تعدد المستخدمين):** عدة عملاء يستخدمون نفس البنية التحتية بشكل معزول.
    

---
### 📌 من يضبط خصائص السحابة؟

1. **المزود (Cloud Provider)** مثل AWS, Azure, Google Cloud:
    
    - هو اللي يبني ويملك البنية التحتية الضخمة (Data Centers, Physical Servers, Network Fabric).
        
    - يوفر لك الأدوات (بوابة إدارة، APIs، خدمات جاهزة).
        
    - يضمن **الأمن المادي + توفر الخدمة + البنية الأساسية للشبكة**.
        
2. **المستخدم (الشركة العميلة / IT team):**
    
    - يضبط الخصائص بنفسه داخل حسابه:
        
        - إعداد **VPC (Virtual Private Cloud)**.
            
        - التحكم في **Security Groups** (من يدخل ومن يخرج).
            
        - بناء الـ **Subnets, Routing tables, VPN/Direct Connect**.
            
    - يحدد إذا بيستخدم **SaaS / IaaS / PaaS** حسب حاجته.
        
    - هو المسؤول عن **التطبيقات والبيانات** (إعداد OS, قواعد البيانات، حسابات المستخدمين…).

---
---

### 🔹 **VNIC = Virtual Network Interface Card**

- مثل **كرت الشبكة (NIC)** اللي في الكمبيوتر العادي، لكن نسخة **افتراضية**.
    
- كل **Virtual Machine (VM)** في السحابة لازم يكون لها VNIC عشان تقدر تدخل الشبكة.
    
- الـ VNIC يحتوي على:
    
    - **MAC Address**
        
    - **IP Address** (خاص/عام)
        
    - إعدادات الشبكة (subnet, security group, routing)
        

---

### 📌 مثال عملي:

- عندك **VM في AWS EC2**:
    
    - يتعطى VNIC تلقائيًا.
        
    - الـ VNIC يربطه بالـ **VPC Subnet**.
        
    - يحدد إذا يقدر يوصل للإنترنت (لو كان عنده Public IP أو Internet Gateway).
        

---

✨ تشبيه:

- **NIC العادي** = كرت الشبكة الفزيائي اللي في اللابتوب.
    
- **VNIC** = نفس الكرت لكن نسخة برمجية داخل السحابة أو VM.
---

---

## 🔹 Deployment Models (نماذج النشر)

1. **Public Cloud**
    
    - السحابة متاحة للجميع عبر الإنترنت (مثل AWS, Azure, Google Cloud).
        
    - الشركة المزودة تدير كامل البنية التحتية.
        
    - المستخدم يدفع على قدر الاستهلاك (pay-as-you-go).
        
    - **أمثلة الاستخدام**: مواقع التجارة الإلكترونية، التطبيقات العامة.
        
2. **Private Cloud**
    
    - بيئة سحابية خاصة بمؤسسة واحدة فقط.
        
    - يمكن أن تكون مستضافة داخل الشركة (On-premises) أو عند مزود خدمة مخصص.
        
    - تعطي **تحكم وأمان أكبر** لكن تكلفتها أعلى.
        
    - **أمثلة الاستخدام**: البنوك، الجهات الحكومية.
        
3. **Hybrid Cloud**
    
    - مزيج بين Public و Private.
        
    - تسمح بمرونة في نقل البيانات والتطبيقات بين البيئتين.
        
    - **أمثلة الاستخدام**: مؤسسة تستخدم سحابة خاصة لحفظ بيانات حساسة، وسحابة عامة للتطبيقات العادية.
        
4. **Community Cloud**
    
    - تشاركها عدة منظمات لها نفس المتطلبات (مثل الجامعات، الهيئات البحثية).
        
    - تقلل التكاليف على الأعضاء لأنها موزعة.
        

---

## 🔹 Service Models (نماذج الخدمة)

1. **IaaS (Infrastructure as a Service)**
    
    - البنية التحتية كخدمة: سيرفرات، تخزين، شبكات.
        
    - العميل يدير الـ OS والتطبيقات، بينما المزود يدير الـ Hardware.
        
    - **مثال**: AWS EC2, Google Compute Engine.
        
2. **PaaS (Platform as a Service)**
    
    - منصة جاهزة لتطوير وتشغيل التطبيقات.
        
    - العميل يدير التطبيقات فقط، أما النظام الأساسي والبنية التحتية يديرها المزود.
        
    - **مثال**: Google App Engine, Microsoft Azure App Service.
        
3. **SaaS (Software as a Service)**
    
    - برامج جاهزة متاحة عبر الإنترنت.
        
    - لا يحتاج المستخدم إلى إدارة أي شيء (فقط يستخدم التطبيق).
        
    - **مثال**: Gmail, Office 365, Dropbox.
        
4. **XaaS (Anything/Everything as a Service)**
    
    - أي خدمة تقدم عبر الإنترنت (Backup as a Service, Security as a Service).
        
    - توسع جديد ليشمل خدمات مختلفة خارج الثلاثة التقليدية.

![[Professor Messer - Cloud Models - CompTIA Network+ N10-009 - 1.3 [wI2x6eGF1Yg - 853x480 - 3m54s](1).png]]

---

## 🔹 ملاحظات مهمة للامتحان

- **Public Cloud = أقل أمان وأرخص**
    
- **Private Cloud = أكثر أمان وأغلى**
    
- **Hybrid Cloud = مزيج ومرونة**
    
- **Community Cloud = مشاركة بين منظمات متشابهة**
    
- **IaaS = VM جاهز لكن تدير OS**
    
- **PaaS = بيئة تطوير**
    
- **SaaS = برنامج كامل جاهز**
---


## 🔹 البروتوكولات المهمة وأنواع الـ IP

- **ICMP (Internet Control Message Protocol):** يُستخدم مع أوامر مثل _ping_ و _tracert_.
    
- **TCP (Transmission Control Protocol):** بروتوكول موثوق، يعتمد على الاتصال (Connection-Oriented).
    
- **UDP (User Datagram Protocol):** أسرع لكن غير موثوق (Connectionless).
    
- **GRE (Generic Routing Encapsulation):** يُستخدم لإنشاء أنفاق VPN.
    
- **IPSec (Internet Protocol Security):** لتأمين البيانات عبر التشفير والمصادقة.
    

---

## 🔹 المنافذ الشائعة (Ports & Services)

|البروتوكول|المنفذ|الوظيفة|

## 🔹 المنافذ الشائعة (Ports & Services)

- **FTP** → Port 20/21 → نقل الملفات
    
- **SFTP / SSH** → Port 22 → نقل آمن وإدارة عبر الطرفية
    
- **Telnet** → Port 23 → إدارة أجهزة عبر النص (غير آمن)
    
- **SMTP** → Port 25 → إرسال البريد
    
- **DNS** → Port 53 → تحويل أسماء المواقع إلى IP
    
- **DHCP** → Port 67/68 → توزيع عناوين IP تلقائيًا
    
- **HTTP** → Port 80 → تصفح الويب (غير آمن)
    
- **HTTPS** → Port 443 → تصفح الويب (آمن)
    
- **NTP** → Port 123 → مزامنة الوقت
    
- **SNMP** → Ports 161/162 → إدارة ومراقبة الشبكات
    
- **LDAP** → Port 389 → إدارة الأدلة (Directories)
    
- **LDAPS** → Port 636 → إدارة الأدلة بشكل آمن
    
- **RDP** → Port 3389 → التحكم بسطح المكتب عن بعد
---

## 🔹 أنواع الترافيك (Traffic Types)

- **Unicast:** من جهاز واحد إلى جهاز واحد (One-to-One).
    
- **Broadcast:** من جهاز واحد إلى كل الأجهزة في الشبكة (One-to-All).
    
- **Multicast:** من جهاز واحد إلى مجموعة أجهزة محددة (One-to-Many).
    
- **Anycast:** من جهاز واحد إلى أقرب جهاز من مجموعة (One-to-Nearest).
    

---

📌 **الخلاصة للامتحان**:

- احفظ البروتوكولات + أرقام المنافذ الأساسية.
    
- فرّق بين TCP (موثوق) و UDP (سريع وغير موثوق).
    
- اعرف أنواع الترافيك الأربع (Unicast, Broadcast, Multicast, Anycast).


---

# **Other Useful Protocols – Security & VPN**

### 🔐 **IPSec (Internet Protocol Security)**

- **وظيفة**: يؤمّن الترافيك على طبقة الشبكة (Layer 3).
    
- يستخدم في VPNs.
    
- يقدم: **Confidentiality, Integrity, Authentication**.
    
- يعتمد على بروتوكولات فرعية: **AH** و **ESP**.
    

---

### 📑 **AH (Authentication Header)**

- يوفر **التوثيق** و **سلامة البيانات** (integrity).
    
- لا يقوم بالتشفير (يعني ما فيه confidentiality).
    
- بروتوكول رقم 51.
    

---

### 🔒 **ESP (Encapsulating Security Payload)**

- يوفر **التشفير + التوثيق + سلامة البيانات**.
    
- الأكثر استخدامًا مع IPSec.
    
- بروتوكول رقم 50.
    

---

### ⚙️ **IKE (Internet Key Exchange)**

- بروتوكول لتبادل المفاتيح وإنشاء الـ **Security Association (SA)**.
    
- يعمل غالبًا مع IPSec.
    
- يمر بمرحلتين: Phase 1 (تبادل المفاتيح) و Phase 2 (بناء النفق).
    

---

### 🛠 **Modes of IPSec**

- **Transport Mode**
    
    - فقط **payload** (البيانات) يتشفّر، الـ IP header يبقى واضح.
        
    - يُستخدم غالبًا بين جهازين نهاية لنهاية (Host-to-Host).
        
- **Tunnel Mode**
    
    - يتشفّر **كل الـ packet** (payload + IP header).
        
    - يُضاف IP header جديد للنفق.
        
    - يُستخدم في **VPNs بين شبكتين** (Site-to-Site).
        

---

### 🌐 **VPNs (Virtual Private Networks)**

- **Site-to-Site VPN**: يربط شبكتين كاملتين عبر الإنترنت باستخدام نفق IPSec (Tunnel Mode).
    
- **Remote Access VPN**: مستخدم فردي يتصل بالشبكة عن بعد (غالبًا عبر SSL VPN أو IPSec).
    

---

### 🌀 **GRE (Generic Routing Encapsulation)**

- بروتوكول نفق عام (Protocol 47).
    
- ما يوفر **تشفير**، فقط تغليف.
    
- ممكن دمجه مع IPSec لإضافة التشفير.
    

---

### 📡 **ICMP (Internet Control Message Protocol)**

- بروتوكول تشخيص (Protocol 1).
    
- يستخدم في ping, traceroute.
    
- ما فيه تشفير أو حماية، لكنه أساسي لفحص حالة الشبكة.
    

---

✅ **خلاصة للمراجعة**:

- IPSec = أساس أمان VPN.
    
- AH = توثيق فقط.
    
- ESP = تشفير + توثيق.
    
- IKE = تبادل مفاتيح.
    
- Transport Mode = جهاز لجهاز.
    
- Tunnel Mode = شبكة لشبكة (Site-to-Site).
    
- GRE = تغليف بدون أمان.
    
- ICMP = تشخيص.

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

![[Pasted image 20251007180610.png]]


---




## (Objective 1.5)

في **Network+ N10-009**، الهدف 1.5 يطلب منك أن **تشرح خصائص وأنواع محولات الإرسال والاستقبال (Network Transceivers)**

---

### 🔹 ما هو الـ Transceiver؟

- كلمة **Transceiver** = **Transmitter + Receiver**.
    
- جهاز مسؤول عن **تحويل الإشارات الرقمية إلى ضوئية أو كهربائية والعكس**، حتى يمكن للبيانات الانتقال عبر الوسيط المناسب (سلك نحاسي أو ألياف ضوئية).
    
- يُستخدم عادةً في المنافذ القابلة للتبديل في **السويتشات والراوترات**.
    

---

### 🔹 وظيفة الـ Transceiver:

1. **الإرسال (Transmit):** يحوّل البيانات من الجهاز إلى إشارة ضوئية أو كهربائية.
    
2. **الاستقبال (Receive):** يستقبل الإشارة من الكابل ويحوّلها إلى بيانات رقمية مفهومة للجهاز.
    
3. **المرونة:** يمكن استبداله بسهولة دون الحاجة لتغيير السويتش بالكامل (Hot-swappable).
    
4. **التوافق:** يدعم وسائط مختلفة مثل الألياف الضوئية (Fiber) أو النحاس (Copper).
    

---

### 🔹 أنواع الـ Transceivers الشائعة:

|النوع|الاختصار|السرعة|الوسيط|المدى|الملاحظات|
|---|---|---|---|---|---|
|**GBIC**|Gigabit Interface Converter|1 Gbps|ألياف|~550 م|قديم وكبير الحجم، استُبدل بـ SFP|
|**SFP**|Small Form-factor Pluggable|1 Gbps|ألياف أو نحاس|حتى 10 كم|الأكثر استخدامًا في شبكات الجيجابت|
|**SFP+**|—|10 Gbps|ألياف|حتى 10 كم|نفس الحجم لكن أسرع|
|**QSFP / QSFP+ / QSFP28**|Quad Small Form-factor Pluggable|40–100 Gbps|ألياف|حتى 40 كم|يستخدم في مراكز البيانات|
|**BiDi (Bidirectional)**|—|1–10 Gbps|ألياف مفردة|حتى 10 كم|يرسل ويستقبل على نفس الليف باستخدام موجتين|
|**RJ-45 Copper SFP**|—|1 Gbps|كابلات Ethernet (Cat 5e/6)|حتى 100 م|لتحويل المنفذ من Fiber إلى Copper|

---

### 🔹 الأطوال الموجية (Wavelengths):

|الطول الموجي|نوع الألياف|الاستخدام|المسافة|
|---|---|---|---|
|**850 nm**|Multimode Fiber (MMF)|مسافات قصيرة|~300–400 م|
|**1310 nm**|Singlemode Fiber (SMF)|مسافات متوسطة|~10 كم|
|**1550 nm**|Singlemode Fiber (SMF)|مسافات طويلة جدًا|~40 كم وأكثر|

---

### 🔹 خصائص إضافية مهمة:

- **Hot-swappable:** يمكن تغييره أثناء عمل الجهاز دون إيقاف التشغيل.
    
- **DDM (Digital Diagnostic Monitoring):** ميزة مراقبة درجة الحرارة، الجهد، والطاقة الضوئية.
    
- **Loopback Test:** لاختبار سلامة المنفذ أو الكابل.
    
- **Compatibility:** لا يمكن خلط MMF مع SMF أو استخدام نوع خاطئ من الموصلات.
    

---

### 🔹 مقارنة سريعة:

| النوع     | السرعة  | المدى     | الوسيط         | قابل للتبديل |
| --------- | ------- | --------- | -------------- | ------------ |
| SFP       | 1G      | حتى 10 كم | Fiber / Copper | ✅            |
| SFP+      | 10G     | حتى 10 كم | Fiber          | ✅            |
| QSFP      | 40–100G | حتى 40 كم | Fiber          | ✅            |
| RJ-45 SFP | 1G      | حتى 100 م | Copper         | ✅            |


---


## .6)

في **Network+ N10-009**، الهدف 1.6 يطلب منك أن **تشرح أنواع البنى المعمارية للشبكات (Network Architectures)**  
وهي الطريقة التي تُصمم وتُنظم بها الشبكة لتحديد كيف تتصل الأجهزة وتتبادل البيانات.

---

### 🔹 **أولاً: أنواع البنى الأساسية (Network Types)**

|النوع|الاسم|الوصف|
|---|---|---|
|**LAN**|Local Area Network|شبكة محلية في موقع واحد مثل مكتب أو مبنى. سريعة (1Gbps–10Gbps).|
|**WLAN**|Wireless LAN|شبكة محلية لاسلكية تعتمد على Wi-Fi.|
|**WAN**|Wide Area Network|تربط مواقع بعيدة عبر الإنترنت أو خطوط مؤجرة (Leased Lines).|
|**MAN**|Metropolitan Area Network|تغطي مدينة أو نطاقًا حضريًا. مثال: شبكة جامعة أو مدينة ذكية.|
|**PAN**|Personal Area Network|تربط أجهزة شخصية (Bluetooth, NFC).|
|**CAN**|Campus Area Network|شبكة تربط عدة مبانٍ ضمن موقع واحد (مثل جامعة أو مجمع شركات).|
|**SAN**|Storage Area Network|شبكة مخصصة لتخزين البيانات ونقلها بين الخوادم وأجهزة التخزين.|

---

### 🔹 **ثانيًا: البنى المعمارية حسب التصميم (Architectural Models)**

1. **Client-Server Architecture (العميل والخادم)**
    
    - الخادم يقدم خدمة (ملفات، طباعة، مواقع ويب...)
        
    - العميل يطلب الخدمة ويستهلكها.
        
    - أمثلة: خوادم البريد، خوادم الويب، خوادم الملفات.
        
    - **مميزات:** تحكم مركزي، أمان أعلى.
        
    - **عيوب:** يعتمد على الخادم، فإذا تعطل تتوقف الخدمة.
        
2. **Peer-to-Peer (نظير إلى نظير)**
    
    - كل جهاز يمكن أن يكون عميلًا وخادمًا في آن واحد.
        
    - تُستخدم في البيئات الصغيرة أو المشاركة البسيطة للملفات.
        
    - **أمثلة:** مشاركة الملفات عبر Windows Workgroup أو تطبيقات مثل BitTorrent.
        
    - **عيوب:** أمان أقل، صعوبة الإدارة في الشبكات الكبيرة.
        
3. **Three-Tier Architecture (ثلاث الطبقات)**
    
    - **Access Layer:** حيث تتصل الأجهزة النهائية (PCs, Printers).
        
    - **Distribution Layer:** يربط بين Access وCore ويتعامل مع السياسات (VLANs, Routing).
        
    - **Core Layer:** الطبقة الأساسية عالية السرعة التي تربط كل شيء.
        
    - تُستخدم في الشبكات المتوسطة والكبيرة لتوزيع الحمل والتحكم.
        
4. **Spine-Leaf Architecture (العمود والأوراق)**
    
    - تصميم حديث في مراكز البيانات.
        
    - **Spine Switches** = النواة الأساسية،  
        **Leaf Switches** = تتصل بالأجهزة والخوادم.
        
    - كل Leaf يتصل بكل Spine مباشرة لتقليل التأخير (Low Latency).
        
    - **ميزة:** لا يوجد عنق زجاجة (Bottleneck)، ويسهل التوسع الأفقي.
        

---

### 🔹 **ثالثًا: بنى الشبكات الافتراضية والحديثة**

1. **Software-Defined Networking (SDN)**
    
    - تفصل بين **Control Plane** (العقل) و**Data Plane** (التنفيذ).
        
    - الإدارة تتم عبر **Controller** مركزي يبرمج السويتشات.
        
    - **ميزة:** تحكم مرن وسهل التوسع، مفيد في مراكز البيانات الكبرى.
        
2. **Cloud-Based Networks**
    
    - تستخدم موارد سحابية بدلاً من أجهزة محلية.
        
    - الأنواع:
        
        - **Public Cloud** (AWS, Azure)
            
        - **Private Cloud** (داخلي للشركة)
            
        - **Hybrid Cloud** (دمج بين الاثنين).
            
    - **ميزة:** خفض التكاليف وسهولة الإدارة.
        
3. **Zero Trust Architecture (ZTA)**
    
    - لا يتم الوثوق بأي جهاز أو مستخدم تلقائيًا حتى داخل الشبكة.
        
    - يعتمد على **التحقق المستمر (Continuous Verification)** و**Least Privilege Access**.
        
    - **هدفه:** تقليل المخاطر داخل الشبكات الكبيرة أو الموزعة.
        
4. **Edge Computing**
    
    - نقل المعالجة من السحابة إلى **حافة الشبكة (Edge)** قرب المستخدم.
        
    - مثال: أجهزة IoT تعالج البيانات محليًا لتقليل التأخير.
        

---

### 🔹 **رابعًا: البنى المعمارية اللاسلكية (Wireless Architectures)**

|النوع|الوصف|مثال|
|---|---|---|
|**Standalone APs**|نقاط وصول مستقلة يتم ضبطها يدويًا واحدة تلو الأخرى.|شبكة مكتب صغيرة.|
|**Controller-based APs**|نقاط وصول تدار مركزيًا بواسطة Wireless Controller.|الشركات الكبيرة.|
|**Mesh Network**|كل نقطة وصول تتصل بالأخرى لتغطية واسعة.|المدن الذكية أو المزارع.|

---

### 🔹 **خامسًا: الشبكات المتكاملة (Converged Networks)**

- شبكة واحدة تنقل **الصوت، الفيديو، والبيانات** معًا.
    
- تعتمد على تقنيات مثل **QoS (Quality of Service)** لتحديد أولوية مرور الصوت أو الفيديو.
    
- أمثلة: VoIP، مكالمات Teams/Zoom عبر نفس الشبكة.
    

---

### 🧠 **نصائح الاختبار (Network+ Exam Tips):**

1. اربط كل نوع من الشبكات بالمجال الذي يغطيه:
    
    - **LAN →** مبنى
        
    - **CAN →** جامعة أو مجمع
        
    - **MAN →** مدينة
        
    - **WAN →** دولي
        
2. احفظ طبقات التصميم الثلاث (Access → Distribution → Core).
    
3. تذكّر أن **Spine-Leaf** = شبكة عالية السرعة تستخدم في **Data Centers**.
    
4. **SDN** يعتمد على برمجة الشبكة من **Controller مركزي**.
    
5. **Zero Trust** = لا ثقة بدون تحقق.

---



## 🧠 الفكرة الأساسية

**SDN – Software-Defined Networking**  
تعني: فصل **التحكم في الشبكة (control)** عن **تمرير البيانات (data)**، بحيث لا يكون السويتش أو الراوتر هو من “يقرر” ويُنفّذ في نفس الوقت، بل تُدار قرارات الشبكة مركزيًا عبر **Controller** ذكي.

---

## ⚙️ بنية SDN

|الطبقة|الاسم|الدور|
|---|---|---|
|**1️⃣ Application Layer**|تطبيقات الإدارة والسياسات|تحتوي على تطبيقات الأمان، المراقبة، أو أتمتة الشبكة (Automation)|
|**2️⃣ Control Layer**|**SDN Controller**|العقل المركزي الذي يتخذ القرارات ويُرسلها للأجهزة|
|**3️⃣ Data Layer**|أجهزة الشبكة (Switches/Routers)|تنفّذ الأوامر فعليًا — أي تمرير الترافيك حسب سياسات الـ Controller|

---

## 🧩 كيف يعمل النظام عمليًا

1. **التطبيقات (Applications)** تقول:
    
    > “أريد حجب هذا البروتوكول عن هذه الشبكة.”
    
2. **الـ Controller** يحوّل هذا القرار إلى أوامر تقنية باستخدام بروتوكولات مثل:
    
    - **OpenFlow**
        
    - **NETCONF**
        
    - **REST APIs**
        
3. **الأجهزة (Data Plane)** تنفّذ الأوامر فورًا بدون أن تحتاج معرفة “السبب”، فقط “كيف تنفذ”.
    

---

## 📡 أنواع الـ Planes في SDN

|Plane|الوصف|
|---|---|
|**Data Plane**|مسؤول عن **تمرير الباكيتات** فعليًا (switches, routers).|
|**Control Plane**|مسؤول عن **اتخاذ القرارات** مثل routing tables.|
|**Management Plane**|مسؤول عن **مراقبة وتعديل إعدادات** الشبكة (مثل CLI, SNMP, APIs).|

SDN يفصل الـ Control عن الـ Data — بحيث تكون الإدارة **مركزية وسهلة البرمجة**.

---

## 🔄 المزايا

1. **مرونة (Flexibility):** يمكنك تعديل سياسات الشبكة برمجيًا بدل الدخول لكل جهاز.
    
2. **أتمتة (Automation):** تغييرات الشبكة تتم آليًا عبر سكربتات أو أنظمة مركزية.
    
3. **رؤية كاملة (Visibility):** الـ Controller يعرف كل التوبولوجي ويضبطها لحظيًا.
    
4. **قابلية التوسع (Scalability):** مثالي لمراكز البيانات الكبيرة والـ Cloud.
    

---

## ⚠️ التحديات

- الاعتماد العالي على الـ Controller (Single Point of Failure إن لم يُنسّخ).
    
- الحاجة إلى مهارات برمجية (Python, REST APIs).
    
- التكامل مع الأنظمة القديمة (Legacy integration).
    

---

## 💡 مثال واقعي

في شبكة تقليدية:

> عندما يزداد الضغط على سويتشٍ ما، عليك يدويًا تعديل الـ VLANs أو الـ routes.

في SDN:

> الـ Controller يكتشف الازدحام ويُعيد توزيع الترافيك تلقائيًا إلى مساراتٍ أقل ازدحامًا — خلال ثوانٍ فقط.

---

## 🧩 تذكّر في الامتحان

| سؤال محتمل                                                | الجواب المختصر                                            |
| --------------------------------------------------------- | --------------------------------------------------------- |
| ما الذي يميز SDN عن الشبكات التقليدية؟                    | **فصل control عن data plane** وإدارة مركزية عبر software. |
| ما دور الـ Controller؟                                    | يتخذ قرارات التوجيه ويرسلها للأجهزة.                      |
| ما البروتوكول الشائع للتواصل بين الـ Controller والأجهزة؟ | **OpenFlow**                                              |
| فائدة SDN؟                                                | تسهيل الإدارة، الأتمتة، والتحكم البرمجي.                  |




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
s

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


sssss