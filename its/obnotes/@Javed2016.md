---
title: **Security in Intelligent Transport Systems for Smart Cities: From Theory to Practice**
authors: Muhammad Awais Javed, Wassim Znaidi
year: 2016
link: zotero://select/items/@Javed2016
---
status: #
links:

## 摘要：

## 重點：

* ITS系統的概念是車輛間無所不在地連結形成一個車聯網(Internet of Vehicles, IoV)(Javed and Znaidi, 2016, p. 1) 
* 資料是由路邊單元(RSU)及各種感測器蒐集而來，感測器可以放置在道路、建築物、人體，以建構成智慧程式 (Javed and Znaidi, 2016, p. 1) 
* ITS的通訊主要有二種模式，一為車輛對車輛(V2V)，另一為車輛對設施(V2I) (Javed and Znaidi, 2016, p. 1-2) 
* 拒絕服務 (DoS),干擾 (jamming), 竄改廣播(broadcast tampering), 中間人攻擊(man in the middle), Sybil, 竊聽與訊息竄改(eavesdropping and message tampering)是少數幾個一般的資通攻擊，對ITS的車輛造成威脅。
* ITS的安全要求包含可用性(availability), 真實性(authenticity), 機敏性(confidentiality), 整體性(integrity) and [[non-repudiation]] of the traffic and mobility data. 
* 美國與歐洲的標準都已臻成熟，提供確實的安全架構與演算法，在這些標準中以橢圓曲線密碼學為基礎的演算法用於數位簽章及ITS訊息加密。特別在數位簽章上，即便橢圓曲線整合加密方案及進階加密標準為預設方法，在加上橢圓曲線數位簽章演算法。
* 防護各種攻擊威脅改善ITS系統的可靠性，卻也造成計算成本，因為將增加封包大小及在傳送端簽章及加密封包造成的時間延遲，及在接受端需要驗證與解密的時間延遲。
* 另一方面也會造成服務品質的遺失。安全與服務品質之間的考量也是ITS的整體一部分
* ITS的核心組成包含車輛(Vehicle)、路邊單元(RSU)、及交通控制中心(TCC)。藉由V2V及V2I通訊可以在ITS核心元件間分享交通及行動資訊。分享的資訊在WAVE標準中稱為基本安全訊息(Basic Safty Message, BSM)，在ETSI標準中稱為協同認知訊息(Cooperative Awareness Messages, CAM)，此外在ETSI標準中還特別定義非集中環境通知訊息(Decentralized Environmental Notification Messages, DENMs)以傳送警告通知。WAVE為Wireless Access for Vehicular Environment美國標準，ESTI為 European Telecommunications Standards Institute歐洲標準，兩種標準都定義ITS應用的完整的網路階層架構包括實體層(MAC/PHY)、網路層(transport and network layer mechanism)、應用層(data traffic at the application layer)、及安全與管理通信協定(security and management procedures)。 收到CAM後，ITS建立區域動態圖(Local Dynamic Map, LDM)，描述周遭交通的資料庫，運用LDM，車輛可以制定關鍵駕駛決策，RSU可以傳送地理警示通知，TCC可以管理程式交通。LDM掌握車輛的交通認知的精準度。

<h1>Annotations
 (8/25/2022, 6:05:08 PM)</h1> 
 
“Security is a key challenge in the implementation of ITS applications. There exist a plethora of security attacks today that can negatively impact the reliability of ITS applications. Particularly, the ITS security requirements include availability, authenticity, confidentiality, integrity and non-repudiation of the traffic and mobility data. Denial of service (DoS), jamming, broadcast tampering, man in the middle, Sybil, eavesdropping and message tampering are few of the common attacks that pose threat to the safety of vehicles in ITS [11–13].” (Javed and Znaidi, 2016, p. 2) its安全需求及一般的資通攻擊 

“ITS standards in US and Europe that have matured over the years now provide concrete security architecture and algorithms. The use of Elliptic Curve Cryptography (ECC) based algorithms have been proposed for digital signatures and encryption of ITS messages in these standards. Specifically, for digital signature, Elliptic Curve Digital Signature Algorithm (ECDSA) is used whereas Elliptic Curve Integrated Encryption Scheme (ECIES) with Advanced Encryption Standard (AES) is the default encryption algorithm [14,15].” (Javed and Znaidi, 2016, p. 2) ECC, ECDSA, ECIES 加密演算法 

“This involves an increased packet size and delay required for signing and/or encrypting packets at the transmitter and verifying and/or decrypting them at the receiver.” (Javed and Znaidi, 2016, p. 2) 

“Another implication of using security in ITS is the loss of safety information” (Javed and Znaidi, 2016, p. 2) 

“Therefore, security and QoS have a trade-off and balancing each of these factors is an integral component of ITS.” (Javed and Znaidi, 2016, p. 2) 

“the impact of security on Quality of Service (QoS) and safety awareness in the context of ITS applications” (Javed and Znaidi, 2016, p. 3) 

“Vehicles form the core component of ITS along with infrastructure road side units and traffic command center (TCC). Using Vehicle to Vehicle (V2V) and Vehicle to Infrastructure (V2I) communications, important traffic and mobility information is shared between different components of ITS. There currently exist two main ITS standards known as Wireless Access for Vehicular Environments (WAVE) [19] and European Telecommunications Standards Institute (ETSI ITS) [20] in United States and Europe respectively. Both of these standards define the complete network layered architecture including the MAC/PHY layer functions, transport and network layer mechanism, data traffic at the application layer, and security and management procedures for the ITS applications.” (Javed and Znaidi, 2016, p. 3) fig1說明 

“Vehicles periodically broadcast their traffic and mobility information with each other and these messages are known as Basic Safety Messages (BSMs) in the WAVE standard and Cooperative Awareness Messages (CAMs) in the ETSI standard. Moreover, the ETSI standard defines a special message for disseminating warning notifications called Decentralized Environmental Notification Messages (DENMs)” (Javed and Znaidi, 2016, p. 3) 

“Using the information received in CAMs, each ITS station develops a local dynamic map (LDM) as shown in Figure 2 which is a database of neighborhood traffic” (Javed and Znaidi, 2016, p. 3) 

“With the help of LDM, vehicles could take critical driving decisions, RSUs could disseminate geographical warning notifications and” (Javed and Znaidi, 2016, p. 3) 

“TCC could manage city level traffic” (Javed and Znaidi, 2016, p. 4) 

“The accuracy of LDM thus holds the key to the precision of traffic awareness of vehicles.” (Javed and Znaidi, 2016, p. 4) 

“Security Threats and Countermeasures” (Javed and Znaidi, 2016, p. 4) 翻譯 

“The key requirements of a secure vehicular network includes availability that guarantees transmission of data within latency requirements using low overhead and light weight cryptographic algorithms. Confidentiality makes vehicle identities and data completely anonymous. Authentication is another key security feature that ensures messages are sent by a legitimate ITS station, the surrounding traffic locations are correctly verified and data attacks from malicious users are prevented. To define proper data access control for different ITS stations, authorization is a vital security requirement. Moreover, data integrity and validation that the data has not been tempered by a malicious user is another security challenge.” (Javed and Znaidi, 2016, p. 4) 

“Denial of Service (DoS) attacks” (Javed and Znaidi, 2016, p. 4) 

“flooding attacks” (Javed and Znaidi, 2016, p. 4) 

“Sybil attacks” (Javed and Znaidi, 2016, p. 4) 

“eavesdropping and data interception are attacks that let malicious users access the sensitive information in the transmitted messages. Encryption is an effective cryptographic solution against such attacks. Vehicle authentication and authorization is compromised by attacks such as falsified entities, cryptographic replication, Global Navigation Satellite System (GNSS) spoofing, and timing attacks.” (Javed and Znaidi, 2016, p. 4) 

“Data Integrity is impacted by attacks such as Masquerading in which a vehicle uses a valid network identifier to broadcast itself as an emergency vehicle and thus effects movement of other vehicles. Another type of attack known as Data Playback attack in which malicious vehicles rebroadcast old messages within the network to generate false vehicle positions. Similarly, data alteration attacks can modify, delete or change the message content to create ambiguity in the network. Digital signature with certificate is a robust mechanism to minimize threats due to these attacks.” (Javed and Znaidi, 2016, p. 5) 

“Security Architecture” (Javed and Znaidi, 2016, p. 6) 

“Security Headers” (Javed and Znaidi, 2016, p. 7) 

“Certificate Format” (Javed and Znaidi, 2016, p. 8) 

“Security Profiles” (Javed and Znaidi, 2016, p. 8) 

“Elliptic Curve Digital Signature Algorithm (ECDSA)” (Javed and Znaidi, 2016, p. 9) 

“Elliptic Curve Integrated Encryption Scheme (ECIES) with Advanced Encryption Standard (AES)” (Javed and Znaidi, 2016, p. 10)

## 相關文獻：



