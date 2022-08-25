智慧型交通系統 (ITS) 是一種未來技術，主要目標是改善道路安全、交通管理和駕駛員舒適度。ITS系統概念是形成車聯網 (IoV) ，使車輛無處不在的連接，從而為他們提供對道路交通的清晰視野。除了車對車連接外，還從基礎設施路邊單元 (RSU) 和放置在道路、建築物和人體上的各種其他感測器收集數據，構成智慧城市典範。收集到的數據傳輸到車輛雲，幫助管理城市交通，確保在緊急情況下的有效預警通知，為車輛的無線收發器提供擁塞控制和安全演算法選擇，並採取措施分析數據質量和準確性。

安全是ITS 的關鍵挑戰。當今存在過多的安全攻擊，可能會對 ITS 應用系系統的可靠性產生負面影響。特別是，ITS 安全要求包括流量和行動資料的可用性、真實性、機密性、完整性和不可否認性。拒絕服務 (DoS)、干擾(Jamming)、廣播篡改(Broadcast Tampering)、中間人(man-in-th-loop)、女巫攻擊（Sybil）[^1]、竊聽和訊息篡改(eavesdropping and message tampering)是 ITS 中對車輛安全構成威脅的少數常見攻擊。

多年來，美國與歐洲的智慧型交通系統標準(ITS Standards)日臻成熟，提供堅實的安全架構與演算法，如以橢圓曲線密碼學(Elliptic Curve Cryptography)[^2]為基礎的加密演算法用來支持數位簽章(digital signatures)及ITS訊息加密。

雖然安全性提高 ITS 系統的可靠性並提供針對各種威脅的防禦，但也帶來運算成本。這涉及在發送器處簽署和/或加密封包及在接收器處驗證和/或解密封包所需的延遲及增加的封包大小。封包大小增加將增加點對點的安全封包延遲及佔據無線通道頻寬，將造成阻塞，特別是在高交通密度情境。在 ITS 中使用安全性的另一個含義是安全資訊的丟失。通常，車輛每秒將接收數百個封包，並且所有數據在接收器端執行安全處理（驗證和解密）都會增加它們的封包延遲。由於對安全封包施加嚴格的延遲要求，將導致網路服務水準(QoS)的降低，進而轉化為 ITS 中較低的車輛安全性。
[@afzalSecurityVehicularAdHoc2020]
----

**安全威脅與反制**
[@williamsIntelligentTransportSystems2008]
----
**ITS安全架構**

------------

ITS攻擊向量

-----
VANET攻擊
[[車輛隨意網路(VANET)]]將是ITS的核心技術，用於連結車輛及未來的自主車輛。VANET由智慧車輛及道路單元(RSU)所組成，RSU藉由不穩定的無線媒介進行通訊。由於隨意特性，VANET將可能遭受攻擊而迫害道路安全性，特別是當車輛根據VANET資料執行關鍵的航行決策時。以下根據Fatih Sakiz及evil Sen的論文，綜整以下針對VANET的攻擊向量
	* Sybil Attack：在此攻擊中，每一個節點(車輛)假裝有多個識別(identity)，造成網路中其他車輛無法驗證接收的資料，是從一輛或多輛車輛而來。攻擊者的目的在於根據他的想法來塑造網路。Sybil攻擊是對VANET最危險的一種攻擊，相當難以偵測。
	* DDoS Attack：發送超過系統可以處理能量的工作要求，造成系統癱瘓及不可用。在VANET，攻擊者嘗試關閉由RSU所組成的網路，停止車輛與RSU之間的通訊。
	* Blackhole Attack：攻擊者節點在隨意協力網路中操控其他節點使資料封包傳遞時通過攻擊者節點，攻擊者藉以丟棄資料封包造成網路中通訊中斷，致使其他的車輛無法接收重要的道路資訊。
	* Wormhole Attack：
	* False Information Attack
	* Fake Location Information
	* Sensor Deception
	* Replay Attack
	* Passive Eavesdropping Attack

-----

[^1]: [女巫攻擊](https://academy.binance.com/zt/articles/sybil-attacks-explained)
[^2]: [橢圓曲線密碼學](https://zh.m.wikipedia.org/zh-tw/%E6%A4%AD%E5%9C%86%E6%9B%B2%E7%BA%BF%E5%AF%86%E7%A0%81%E5%AD%A6)
