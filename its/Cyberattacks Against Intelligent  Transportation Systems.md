[National ITS Architecture Security]([National ITS Architecture.pdf](file:///E:/Research/ITS%E8%B3%87%E5%AE%89/National%20ITS%20Architecture.pdf))
[FRAME](FRAME)
Japanese ITS System Architecture
[MITRE ATT&CK](https://attack.mitre.org/)
[Transportation Systems Sector Cybersecurity Framework Implementation Guidance](https://www.cisa.gov/sites/default/files/publications/tss-cybersecurity-framework-implementation-guide-2016-508v2_0.pdf)

### ITS 的六大應用子系統 (A&S)

車輛（如汽車、卡車、巴士…等）是運輸系統的基本元件，車輛配置網際網路及具備無線區域網路，使它可與其他車輛分享網際網路，更進階的連結車可以運用各種技術，如光學雷達、雷達、GPS、及3D攝影機，偵測環境及進行無人導航。

道路狀況回報
道路操作員需要不斷地監控交通及目前道路狀況，使用策略設置在道路上的陣列攝影機與感測器，這些裝置傳回即時資料至控制中心，資料包含巴士道路攝影機，速度攝影機，道路天氣站台，及車輛偵測系統。

交通流量控制
道路操作員監控即時的交通及道路狀況，並運用蒐集的資料，介於各種車流控制機制，如交通號誌控制系統，平交道柵欄，動態訊息標誌，及自動閘道系統等，來管理交通流量。

付款應用系統
運用RFID付款設備、付款機臺機制(Kiosk payment)、及電子票證(e-ticket)應用以降低成本增加盈餘。

管理應用系統
ITS神經中心架設、監控、操作ITS的控管系統，包括街燈控制、災害管理、資料與資儲存管理、緊急車輛、及交通與壅塞管理。

通訊應用系統
在ITS運作過程資料扮演重要角色，經由資料蒐集可以使交通流量有效率，可以改善道路安全性，可以增加營收，降低生態與環境衝擊。同時，資料也可由ITS的使用者產生以改善使用經驗，如使用智慧應用程式，社群媒體，及路障與安全事件警告。

-----


11 Real-World ITS Attacks

攻擊者分類

------
### ITS攻擊向量

**實體攻擊**
* 實體連結到曝露的端口，如USB、PS2、序列型端口...等
* 在裝置上使用暴力法或猜測密碼憑據
* 刺探裝置與後端間的網路傳輸
* 掃描保護/關閉的網路以探究網路架構
* 在被破壞的ITS裝備/系統上刪除檔案
* 盜取韌體以回復密碼憑據及組態
* 使用曝露的線路/電纜進行中間人攻擊(Man-in-the-Middle)以攔截資料
* 實體篡改裝置偷取/破壞資料，修改裝置
* 連接一個可移除的儲存裝置，藉由安裝惡意程式
* 傳送不正常的指令到控制及後端伺服器
* 中間人攻擊至後端伺服器的通訊及傳送假資料
* 選取一個ITS裝備作為可信任的進入企業網路的端點
* 運用軟體、硬體、通信協定、作業系統的漏洞弱點
* 可信任的操作員使用權限篡改及破壞裝置

**無線通訊攻擊(V2V, V2I, I2I無線通訊將給予攻擊者機會)**
* V2V, V2I, I2I欺騙訊息傳送影響ITS系統各個層面
* 刺探無線傳輸，如使用車輛的wifi
* 遠端傳送及安裝惡意軟體
* 對於擾亂作業的無線傳輸的電子干擾
* 無線傳輸的中間人攻擊以攔截及/或更改資料
* 運用軟體、硬體、通信協定、作業系統的漏洞弱點
* 運用車輛wifi作為控制器區域網路匯流排(CAN)進入點，再進入車輛線上診斷器(OBD)，遠程訊息處理控制單元(TCU)，及車輛上資訊單元（IVI)
* 經由受損的CAN匯流排對於車輛控制進行遠端劫持
* 在車輛資訊系統中安裝惡意的第三方應用程式
* 經由安裝在與車輛wifi連結的電話上的惡意應用程式攻擊
* 對車輛安全系統的電子干擾，如雷達，聲納等

**網路攻擊(藉由網路產生的資安攻擊，如暴露於Internet連結的IoT，IoT搜尋引擎-[shodan](https://www.netadmin.com.tw/netadmin/zh-tw/technology/2CD1DAA23ECE4C389F0E79EC46396676))**
* 識別與濫用裝備的錯誤配置
* 利用舊軟體與硬體的漏洞弱點 
* 發現與濫用遠端系統，如使用shodan搜尋引擎
* 在系統安裝惡意/間諜程式
* 複雜的國家資助目標定位攻擊或進階持續性威脅(APT)
* 上傳及安裝惡意韌體
* 社會工程攻擊，如魚叉式網路釣魚
* 在網際網路暴露的ITS架構及後端伺服器發動DDoS攻擊
* 運用軟體、硬體、通信協定、作業系統的漏洞弱點
* 暴力法解密及濫用弱身份驗證機制
* 經由廣告、橫幅、假廣告注入惡意程式腳本
* SQL指令注入攻擊(SQL Injection Attacks)
* 跨站腳本攻擊(XSS Attacks)
* 連線劫持攻擊(Session hijack Attacks)
* DNS欺騙及劫持攻擊
* 水坑攻擊(watering hole attacks)
* 內網滲透(pass the hash attacks)
* 票證傳遞攻擊(pass-the-ticket attacks)
* 傳送不正常指令給控制器及後端伺服器
* 選取一個ITS裝備作為可信任的進入企業網路的端點
* 可信任的操作員使用權限篡改及破壞裝置
* 破壞一個第三方合約者電腦，並經由這些受感染的機器進入企業網路運作

-----
### VANET攻擊
[[車輛隨意網路(VANET)]]將是ITS的核心技術，用於連結車輛及未來的自主車輛。VANET由智慧車輛及道路單元(RSU)所組成，RSU藉由不穩定的無線媒介進行通訊。由於隨意特性，VANET將可能遭受攻擊而迫害道路安全性，特別是當車輛根據VANET資料執行關鍵的駕駛決策時。以下根據Fatih Sakiz及evil Sen的論文，綜整以下針對VANET的攻擊向量

* Sybil Attack：在此攻擊中，每一個節點(車輛)假裝有多個識別(identity)，造成網路中其他車輛無法驗證接收的資料，是從一輛或多輛車輛而來。攻擊者的目的在於根據他的想法來塑造網路。Sybil攻擊是對VANET最危險的一種攻擊，相當難以偵測。
* DDoS Attack：發送超過系統可以處理能量的工作要求，造成系統癱瘓及不可用。在VANET，攻擊者嘗試關閉由RSU所組成的網路，停止車輛與RSU之間的通訊。
* Blackhole Attack：攻擊者節點在隨意協力網路中操控其他節點使資料封包傳遞時通過攻擊者節點，攻擊者藉以丟棄資料封包造成網路中通訊中斷，致使其他的車輛無法接收重要的道路資訊。
* Wormhole Attack：二個以上的受損節點依據他們所知的到任何目的地的最短路徑假通知，盡可能地發出路由要求。攻擊者的目的要修改網路的邏輯拓撲使所有路由要求經過他們，以致於可以蒐集與/或操控大量的網路交通訊息。
* False Information Attack：VANET車輛運用其他車輛或RSU生產生或傳遞的資料。這些接受/傳遞的資料不一定是真實的，攻擊者車輛可以產生假資料及傳送至VANET。一般假資訊攻擊包括
	* Fake Location Information：車輛可能廣未假位置資訊，這是一個嚴重問題因為與安全性相關的應用程式/系統依賴精確的車輛位置資料，假資料造成不正確的反應。同時，當封包傳遞至虛幻車輛(Phantom vehicles)時，假位置資訊將造成資料封包遺失。
	* Sensor Deception：藉由模擬假駕駛狀態，攻擊者可以欺騙車輛內的感測器，如在短不不斷地煞車，攻擊者可以模擬路上的交通壅塞，以及車輛可以不正確地廣播交通壅塞的訊息。
* Replay Attack：訊息延後儲存及廣播致使欺騙網路其他節點。攻擊中，重播的訊息不再有用及真實。攻擊者的目的重製及利用原訊息傳送時的狀況藉由重復廣播被儲存的訊息。
* Passive Eavesdropping Attack：監控網路以追蹤車輛移動或收聽他們的通訊。攻擊節點簡易地攔截及檢查網路中流動的訊息。攻擊者的目的是蒐集車輛及通訊模式的資訊以便作為未來攻擊

-----

### 曝露網際網路的ITS裝置

曝露網際網路的ITS裝置是每天都要面對的資安漏洞，可能遭受DDoS的攻擊，這些裝置可以被IoT搜尋引擎如Shodan搜獲。以下討論針對在Shadon搜尋引擎探討發覺曝露網際網路的ITS架構。
當在Shadon輸入「NTCIP」(National Transportation Communications for Intelligent Transportation System Protocol)，發現在美國63個與NTCIP相關的線上裝置。裝置屬於交通號誌控制器或動態訊息號誌控制器，經由無線網路設備連接網際網路，單位名稱是ISP提供商，而非設備操作單位。值得一提示上述兩種設備的產應商上述兩種設備的產品供應商被未顯示資安漏洞。操作單位可以設定控制裝備經由網際網路存取它們。

![[Pasted image 20220729145053.png]]
（Access: 2022/7/29）

如果以供應商來搜循，例如Wanco，一家高速公路與交通控制產品商，可以發現89筆Wanco訊息板的線上資料，裝置經由無線設備（如RomPager  v4.01, Romv4.34, 及更老版本）連上網計網路，這些連網設備都被稱為「Misfortunr Cookie漏洞所利用。單位名稱是ISP提供商，而非設備操作單位。並無發現Wanco的產品有資安漏洞。但如果RomPager的漏洞並未被補救，怎攻擊者可能經由連網設備進行破壞。

曝露網際網路的ITS裝置並非指系統被破壞，但可能造成系統設定不安全。另一角度來看，由於暴露在網際網路上，系統很容易受到攻擊。我們還發現，犯罪者可以利用無線連網設備中已知的漏洞來潛在地訪問和破壞連接的 ITS 設備。

### ITS生態系統風險模型

**定義嚴重影響等級（Impact Severity Level, ISL）**
	* L1 -- 應用系統直接影響大眾安全性及關鍵作業
	* L2 -- 應用系統影響每日運作及收益作業
	* L3 -- 應用系統,支援L1及L2，及組織

**ITS元件與ISL關聯性**
![[Pasted image 20220802100709.png]]
![[Pasted image 20220802100825.png]]
![[Pasted image 20220802100802.png]]


### DREAD威脅模型
[[DREAD威脅模型]]對於ITS保全性提出結構化方法來描述產生可能最高等級的影響：
* Damage potential (損壞可能性)
* Reproducibility (攻擊重現性)
* Exploitability (攻擊發動性)
* Affected users (人員影響性)
* Discoverability (攻擊發現性)

![[Pasted image 20220802100916.png]]

**風險等級**
* 高風險：12-15
* 中風險：8-11
* 低風險：5-7

### ITS資通攻擊風險評量表
根據ITS六大應用子系統與可能的攻擊向量產生的威脅進行評估
車輛
![[Pasted image 20220802101301.png]]

路況
![[Pasted image 20220802101317.png]]

交通流量控制
![[Pasted image 20220802101334.png]]

付款子系統
![[Pasted image 20220802101358.png]]

管理子系統
![[Pasted image 20220802101414.png]]

通訊子系統
![[Pasted image 20220802101426.png]]

風險評估結果觀察
* 對於所有威脅攻擊的評估，高風險佔53.85%，中風險佔40%，低風險佔6.15%
* 針對高風險威脅71.4%屬於網路攻擊，31.4%屬於無線攻擊，25.7%屬於實體攻擊，有部份包含多類型攻擊，這是因為部份裝備及功能可能遭受實體、無線、或網路的複合式攻擊。
* 針對暴露的資通基礎設施的DDoS攻擊，無線傳輸電子干擾，漏洞利用，及暴力破解密碼憑證在DREAD模型下都列為高風險。除了電子干擾，其他的攻擊向量一般用於每日的資通攻擊，所以對於攻擊者使用嘗試測試方法(tried-and-tested)不要驚訝。
* 隔空安裝惡意韌體、遠端綁架車輛控制、傳送不正確/不正當指令至ITS裝置、傳送欺騙的V2I與V2V訊息在DREAD模型下都列為中或低風險，因為這些攻擊都不太容易實施，攻擊者必須具備高超的技能與相關知識才有成功攻擊的可能。
* 值得注意，利用受損的ITS裝置作為企業網路的進入點被認為是中風險，這是因為需要專家等級的計能及破解企業的資安防護才能達成。
* 在ITS六大應用系統中，發現交通流量控制系統及付款應用子系統包含很多威脅，因此列為高風險。


### ITS生態系統保全
防護複雜的ITS生態系統是一件非常困難的任務。根據威脅模型的分析結果可知，網路攻擊對ITS造成最大的攻擊威脅，其次是無線攻擊，最後的實體攻擊。攻擊者可來自國家支助的駭客，犯罪組織，駭客團體，恐怖份子，及內容員工，當然有各種不同的攻擊的原因。資通攻擊與資料洩漏的防護應該是企業每日運作的一部分。終究，對於堅定的對手，沒有任何防禦措施是堅不可摧的
資通攻擊和資料洩露是不可避免的。因此，具備有效的警示，遏止作為，及降低風險流程對於ITS整體防禦是關鍵的。

> ==重要的防禦原則是假設遭受攻擊，實施反製作為==

* 快速評估與反應正在進行中的資安破口
* 遏制安全破口並阻止敏感資料的遺失
* 經由保護所有可利用的途徑先發製人地防止攻擊
* 應用經驗教訓，進一步加強防禦並防止重複事件

![[Pasted image 20220802105750.png]]
ITS安全防護概念圖

**ITS安全防護的技術**
* 網路分段 (Network segmentation)
* 防火牆 (Firewalls)
* 下世代防火牆/統一威脅管理閘道 (Next-generation firewalls/Unified Threat Management (UTM) gateways)
* 防毒軟體 (Anti-malware)
* 反釣魚解決方案 (Anti-phishing solutions)
* 破口偵測系統 (Breach Detection Systems, BDS)
* 入侵防護偵測系統 (IPS/IDS)
* 編碼技術 (Encryption technologies)
* 弱點掃瞄 (Vulnerability scanner)
* Shadon掃瞄 (Shodan scanning)

**ITS防護政策建議**
ITS 生態系統本質上是一個龐大的工業物聯網 (IIoT) 運行環境。各級政府的決策者與 ITS 行業合作，正在積極制定有關運營、技術、互動、安全和保安等的政策和立法。以下為一些對 ITS 的安全可靠運作至關重要政策建議
* 各國正在積極致力於定義和建立自己的 ITS 架構，以滿足其獨特的未來交通需求。陸地相鄰並擁有交通溝聯的國家（例如，公路、鐵路、水路）應相互協調，建立工作小組來定義一個通用、安全和可相互操作的 ITS 架構。如此一來，鄰國就不必承擔試圖整合彼此不兼容的 ITS 架構。歐洲 ITS 架構規範就是一個很好的例子。
* ITS 架構開發必須包括資通安全要求以保護 ITS 生態系統。在當今智慧型裝置互聯的環境下及破壞性資通攻擊數量不斷增加的情況下，ITS 資通安全防護是具強制性的。
* ITS 的關鍵運營要求之一是車對車 (V2V)、車對基礎設施 (V2I) 和基礎設施對基礎設施 (I2I) 通信。因此，需要為 ITS 定義標準化的安全通信協定。升級現有的通信協議系列將比開發全新的通信協議更具成本效益。此外，ITS 需要多種協訂來處理，如低帶寬、高帶寬、短距離、長距離、廣播、多播、一對一和其他通信。
* ITS 生態系統將產生大量的日常用戶資料。這些資料需要安全儲存，並且需要定義和執行嚴格的資料存取使用策略，以保護所有道路用戶的隱私和權利。
* 應起草立法來定義自動駕駛汽車的允許運作界線。這些操作界線應包括責任影響政策、事故協議、自動駕駛汽車允許的道德行為、資料收集和記錄、通信、與其他道路使用者的互動等。
* 應起草立法，規定新的 ITS 裝置、建築和道路車輛在獲得可行駛批准之前必須滿足的最低安全標準（網路和實體）。此外，還必須建立一個認證小組和認證過程，並將其組織起來。

**附件**

車輛連結的技術
* GPS — 全球定位系統 (GPS) 是以地理位置為基礎的導航裝置，全球導航衛星網路提供地面GPS接受器地理位置及時間資訊。連結的車輛使用GPS定位車輛精度達2公尺範圍。
* RADAR — 雷達距離偵測源自軍用科技。微米波雷達(Millimeter Wave Radar, MMW) 是雙頻(Ka- and W-Band)單脈波(mono-pulse)追蹤雷達。MMW安裝在車輛前端保險上，具有多項功能，如前向避碰及交通感應巡航定速(Adaptive Cruise Control, ACC))
* Ultrasonic sensors — 超音波感測器監控車輛前後端目標及警示駕駛人有關可能碰撞的物體，同時也提供自動停車及停車位偵測功能。自動或半自動停車時的車輛運動控制來自超音波的資訊。
* Stereovision cameras — 3D影樣攝影機安裝於擋風波璃，在自動或半自動駕駛時，視覺化辨識車輛週邊，辨識的物件包括車道、交通號誌、紅綠燈、其他車輛，行人...等。
* Lane Keep Assist (LKA) — 車道維持輔助系統具備攝影機可偵測車輛偏離車道，LKL將自動修正方向盤改正車輛航向，並保持車輛在車道內。
* Telematics and OTA services — 遠端訊息服務提供駕駛人道路、交通壅塞、路障、交通事故警示、路況協助、及電子電話(eCall)。隔空(Over-the-Air, OTA)服務可提供更新乳體，更新設定，甚至提供訊息系統的解密鑰匙。遠端訊息及OTA是藉由GPRS, 3G, 或 4G/LTE來實施。

自動車技術
* LIDAR — 光學雷達，顧名思義就是利用雷射脈波及脈波時距來計算距離，是一種光學測距感測器，此種測距裝置可以在任何天候中偵測路上物件。LIDAR一般用於巡航定速與避碰偵測。 
* Infrared headlamps — 紅外線頭燈提供夜間視線而不會干擾其他駕駛人眼睛，紅外線訊號光束可以被紅外線攝影機接收，可用於辨識行人及路上的物件。 
* V2V and V2I communications — 未來連結的車輛及智慧型基礎設施將會以隨意方式(ad-hoc)強制相互通訊，以提供位置、安全警示(如通過十字路口)、及週邊交通等資訊。通訊媒介將使用3G, 4G/LTE, 802.11g/n/p, 802.16...等。無線通訊標準及訊息格式仍在被定義中。

路況回報技術
* Bus lane cameras — 大多數大中型城市都有公車專用道系統，在交通高峰時段優先考慮公交車輛。城市使用公車專用道攝影機(Bus lane cameras)對違規者進行拍照/錄影，並對他們處以罰款。
* High Occupancy Vehicle (HOV) lane cameras — 在交通高峰期，高乘載專用道(HOV lanes)是為有兩個或兩個以上乘員的車輛保留的。高速公路上也有固定的 HOV 車道。城市使用攝影機網路強制執行 HOV 車道，HOV網路攝影機(HOV lane cameras)拍攝違規者的照片/錄影並對其處以罰款。 
* Red light cameras — 紅燈照相機放置在交通路口，以減少碰撞次數。這些照相機拍攝故意闖紅燈的車輛的照片/錄影，市政府會對其處以罰款。 
* Speed cameras — 超速攝影機用於監控車輛是否遵守公佈的速度限制。該系統有一個內置的雷達，可以測量車速。超影機會拍攝違規者的照片/錄影，城市會對他們處以罰款。 
* Railway crossing cameras — 平交道攝影機用於監控平交道交通狀況，這些攝影機的操作類似於紅燈和測速攝影機的組合。當攝影機檢測到事件時，將車輛資訊發送到控制中心進行驗證。控制中心可能會對違規車輛處以罰款或採取其他措施。
* Automatic Number Plate Recognition (ANPR) — 自動車牌辨識(ANPR)技術用於發出自動罰款、停車執法、收費、過境等。
* Induction loop — 電磁感應線圈系統(Induction Loop System)是一種電磁車輛檢測系統，當車輛停在其上時會產生電流。感應迴路通常放置在十字路口，以向交通信號燈發送控制信號。
* Vehicle detection systems — 車輛偵測系統具備有不同類型的功能、準確性和多功能性，例如：速度、車輛數量、車輛分類、停止車輛檢測、錯誤方向車輛、事故檢測，以及其他交通資料，例如佔用率、車輛間距、隊列檢測等。這些數據由中央控制用於交通流量監控。
* UAV road monitoring — 無人機(Unmanned Aerial Vehicles, UAVs)越來越多地用於民用應用。未來，交通控制中心將使用無人機來監控交通並在遠程道路位置執行規定。 
* Roadside weather stations — 道路天氣資訊站測量路面溫度、水膜厚度、氣壓、溫度等環境變量。提供有關當前道路狀況的精確資訊，然後中央控制系統使用這些資訊來做出安全決策。
* Emissions/Air quality sensors — 空氣排放品質用於測量道路級別的空氣品質。從健康和安全的角度監測空氣品質非常重要，尤其是在交通繁忙、人口過剩、大型製造區域、商用車流量大等城市。
* Vehicle location tracking (藉由 GPS, V2I, 目視..等) — 未來的 ITS 基礎設施將支持 V2V 和 V2I 通信，回報車輛位置以改善道路安全。目前，可以通過 ANPR 攝影機進行車輛追踪。商用車輛具有 GPS 追踪器，可向公司車隊控制中心報告車輛位置。

交通流量監控技術
* Reversible lanes — 根據頂端信號顯示(綠色箭頭或紅色十字)，交通可能向任一方向行駛。可逆車道(Reversible lanes)用於改善高峰時段的交通流量。
* Railway crossing barriers — 降低公路與鐵路交叉口前的實體屏障(Railway crossing barriers)，以防止火車接近時車輛移動。這些障礙由鐵路軌道的開關控制。
* Dynamic message signs — 在道路路表標架上方安裝電子交通標誌，用於向通行者顯示重要信息。這些標誌用於顯示有關交通壅塞、事故或事件、道路工程、限速、等待時間、車道信號等的資訊。
* Dynamic road surface markers — 用於動態顯示車道標記的路面 LED 標記。可用於調用逆流車道、標記人行穿越道、標記路肩、添加車道，或在惡劣天氣下提高車道能見度。
* Dynamic road barriers — 與可逆車道信號、鐵路岔道控制、收費系統等結合使用，以降低或提高改變交通流量的實體閘門。
* Traffic signal control systems — 交通號誌控制系統設置於十字路口，以協調和控制十字路口的交通燈號。交通信號燈經由道路嵌入式感應迴路或路邊感測器和探測器發出的控制信號進行操作；信號通過公共 IP 網路或 VPN 從中央控制發送的信號；或以預設的時間間隔傳遞。
* Ramp meter — 閘道儀控(Ramp meter)是一個交通信號燈（僅限紅色和綠色）以及一個信號控制器，可根據當前交通狀況調節進入高速公路的交通流量。使用匝道計，管制汽車進入高速公路以減少過度壅塞。
* Pedestrian detectors — 行人偵測器安裝在十字路口和人行道上，利用其攝影機和感測器於檢測行人。行人檢測系統控制交通信號燈或行人警告燈，例如閃光信標。
* Bicyclist detectors — 自行車騎士偵測器類似於行人檢測器。檢測器使用攝影機和感測器(例如紅外線)來識別騎自行車的人並將控制信號發送到交通燈號控制系統。
* Automated toll collection systems — 自動收費站系統是一些動態閘門，允許車輛在支付通行費後通過。自動收費站系統控制收費公路上的交通流量。(不包括使用 ANPR 為車輛計費且沒有門禁控制的自動收費系統)。
* Emergency vehicle priority system — 緊急車輛優先系統允許緊急車輛，如救火車，救護車，及警車，可以根據響應緊急事件的逕行路徑自動啟動交通號誌時序。經過道路清除使緊急車輛可以快速反應事故。 
* Transit signal priority (TSP) — 大眾運輸號誌優先系統是一組操作改進，通過延長綠燈或縮短紅燈來減少交通車輛在交通號誌處的等待時間。TSP 可以在單一交叉路口、跨走廊或整個街道系統實施。
* Safety systems for autonomous vehicles — 自動駕駛車輛安全系統是一個沿道路設置的雙向 V2I 通信網路，為自動駕駛車輛提供道路、交通、位置和其他重要資訊。自動駕駛汽車可以根據接收到的資訊改變速度、車輛間隙和行駛路線。
* Dedicated lanes for autonomous vehicles — 為實現自動駕駛汽車，在引入的第一階段將為自動駕駛汽車設置專用車道。這些車道將使用動態訊息標誌、動態路面標記、閘道儀控和閘門控制來強制執行。

付款應用系統技術
* Reversible lanes — 根據框架頂顯示的信號（綠色箭頭或紅色十字），交通可能向任一方向行駛的車道。可逆車道(Reversible lanes)用於改善高峰時段的交通流量。
* Railway crossing barriers — 降低平交道實體屏障，，以防止火車接近時車輛移動。這些屏障由鐵路軌道的開關控制。
* Dynamic message signs — Are above roadway gantry mounted electronic traffic signs for displaying important messages to travelers. These signs are used for displaying messages about traffic congestion, accidents or incidents, road works, speed limits, wait times, lane signals, etc. 
* Dynamic road surface markers — These are in-pavement LED markers that are used for dynamically delineating lane markings. They can be used to invoke contraflow lanes, mark pedestrian crossings, mark shoulders, add lanes, or improve lane visibility in bad weather. 
* Dynamic road barriers — Work in conjunction with reversible lane signals, railway switch controls, toll collection systems, etc., to lower or raise physical gates that change the traffic flow. 
* Traffic signal control systems — Are placed at intersections to coordinate and control the intersection’s traffic lights. Traffic lights are operated via control signals sent from road-embedded induction loops or roadside sensors and detectors; via signals sent from the central control over a public IP network or over VPN; or at preset time intervals. 
* Ramp meter — Is a basic traffic light (red and green only) together with a signal controller that regulates the flow of traffic entering freeways according to current traffic conditions.41 The regulated ingress of cars into the freeway using ramp meters reduces excessive congestion. 
* Pedestrian detectors — Installed at intersections and crosswalks, uses a combination of cameras and sensors to detect pedestrians. The pedestrian detection system controls traffic lights or pedestrian warning lights, e.g., flashing beacons. • Bicyclist detectors — Are similar to pedestrian detectors. The detector uses a combination of cameras and sensors, such as infrared, to identify bicyclists and sends control signals to the traffic light control system. 
* Automated toll collection systems — These are dynamic gates that allow vehicles to pass after paying toll. They control traffic flow on tolled roadways. (This excludes automatic toll collection systems that use ANPR to bill vehicles and have no gate controls.) 
* Emergency vehicle priority system — Allows emergency vehicles, e.g., fire trucks, ambulances, and police vehicles, to automatically trigger traffic light sequences along the most direct route when responding to an emergency. By clearing the path ahead, emergency vehicles can respond more quickly.42 57 | Cyberattacks Against Intelligent Transportation Systems: Assessing Future Threats to ITS 
* Transit signal priority (TSP) — Is a set of operational improvements that reduce wait time at traffic signals for transit vehicles by holding green lights longer or shortening red lights. TSP may be implemented at individual intersections, across corridors, or entire street systems.43 
* Safety systems for autonomous vehicles — This is a two-way V2I communication network setup along the roadway to provide autonomous vehicles with road, traffic, location, and other important information. The autonomous vehicles can change speed, in-between vehicle gaps, and travel routes based on the information received. 
* Dedicated lanes for autonomous vehicles — For autonomous vehicles to become a reality, in the first stage of introduction there will be dedicated travel lanes for autonomous vehicles. These lanes will be enforced using dynamic message signs, dynamic road surface markers, ramp meters, and gate controls.

管理應用子系統技術
* Streetlight controls — Management system for outdoor lighting. Streetlights are normally controlled by ambient light sensors or timers, but the ITS control center can monitor and control streetlights individually or in groups. A streetlight management system helps conserve energy, reduces costs, simplifies maintenance, and allows for centralized monitoring. 
* Disaster management — These are a set of procedures activated by the ITS control centers when disaster strikes a municipality. Disasters could be natural calamities, freak accidents, terrorist attacks, etc. Disaster management will typically include opening evacuation routes, plans for first responders, public communications plans, and such. 
* Information sharing services — The ITS ecosystem generates massive amounts of data daily. This data is used across multiple departments for traffic management, for billings, for planning and policy decisions, for creating maintenance schedules, etc. ITS control centers, which are the data collection points, have data sharing services setup for secure and easy access to the data. 
* Data management and storage systems — To process and store big data the ITS ecosystem generates, the control center needs to maintain large data centers. ITS data must be protected and access controlled, so as not to breach user’s privacy rights; for example, no one should be able to track a person’s vehicle movements without legal authorization. 
* Smart parking management — Remote-sensing devices in parkades monitor available spaces and share that information with connected cars, mobile apps, and dynamic signage. Parkades in the near future will coordinate available parking spaces to maximize utilization and revenue. 60 | Cyberattacks Against Intelligent Transportation Systems: Assessing Future Threats to ITS 
* Billing and toll administration — All types of daily transactions, e.g., parkade payments, dynamic tolling, congestion zone charges, ANPR payments, ticket payments, etc., need to be processed quickly and accurately. Billing systems can directly impact traffic flow control mechanisms such as entry gates at tolled bridges and highways. 
* Transit vehicle management — Tracks the real-time position of transit vehicles and uses that information to update/create route schedules and maintenance schedules, identify operational deficiencies, etc. The real-time position and expected arrival time information are made available at bus stops, on the web, on transit apps, and such. 
* Emergency vehicle management — System used by dispatchers to track, route, and quickly send help to the location of the emergency. The system will give traffic signal priority to emergency vehicles at intersections so they can safely reach their destination in the shortest possible time. 
* Traffic and congestion management — These systems control reversible lanes, dynamic road surface markers, dynamic message signs, intersection traffic lights, and such. These are the most important systems in the ITS ecosystem because they are used for managing/controlling the traffic flow of the entire roadway network. 
* Smart traffic light control systems — Are a subsystem of traffic and congestion management. Traffic lights communicate with the ITS control center over a public IP network or over VPN. The control center can change the traffic signal behavior to give priority to emergency and traffic vehicles, or change the traffic signal behavior altogether as the situation demands. 
* Commercial vehicle operations — These are systems run by freight companies to keep track of their fleet. The system tracks vehicle locations, does delivery scheduling and routing in the most efficient manner, processes all required clearance paperwork including for border crossings, manages payment of toll and other surcharges, etc. The system is designed to improve operational efficiency, reduce costs, and increase revenue. When autonomous trucks start driving on the road, these systems will be used to coordinate road trains for super density operations. 
* Maintenance and construction management — Roadways and their supporting infrastructure are in need of regular maintenance, and new roadway constructions are always in the planning pipeline. Engineering depends on ITS data to plan and schedule repairs and identify new construction opportunities. 
* Cooperative traffic and position sharing systems — In the future, connected cars and autonomous vehicles will be ad-hoc sharing their location with each other and with road infrastructure. The ITS ecosystem will need to process received vehicle location data in real-time and share it with the rest of the roadway network and the other nearby connected vehicles. This location data will be used for safety improvement and for traffic flow control. 61 | Cyberattacks Against Intelligent Transportation Systems: Assessing Future Threats to ITS 
* Artificial intelligence (AI) and machine learning (ML) applications — AI and ML applications aim to extract value from big data. For ITS, the goal for AI and ML will be to improve system efficiency, traffic flow prediction models, and disaster response modeling, identify future construction opportunities, create new revenue generation models, improve city expansion modeling, reduce cost, etc. This data analysis is crucial to both city planners and government decision-makers. 
* Road-based location services for autonomous vehicles — To improve the location accuracy of autonomous vehicles, the ITS ecosystem will have land-based GPS transmitters. These transmitters will transmit their exact location as well as other data including traffic, accident/incident information, weather, etc.

通訊應用子系統技術
* Smart apps — The global median for smartphone ownership is 43% and in developed countries, that number increases to more than 50%.44 ITS apps, running on smartphones, are making it easier for users to pay for and use various ITS services. Apps are currently being used for: transit, e-tickets, traffic, car sharing, freight hailing, taxi/limo hailing, parking, trip planning, ride sharing, vehicle diagnostics and management, etc. 
* Social media — A growing size of the population receives their daily news from social media platforms like Twitter and Facebook. ITS operators routinely update the public with important information such as transit delays, strikes, etc., through social medial platforms. 62 | Cyberattacks Against Intelligent Transportation Systems: Assessing Future Threats to ITS 
* Company website — In conjunction with social media, company websites also host important user information for ITS services. Additionally, the websites provide services like trip planning, ticket purchase, fine payments, schedules, etc. • Advertisements — Are one of the major revenue streams for ITS providers. Digital advertisements on display screens are slowly supplanting the traditional print and poster advertisements, although print and posters are not expected to disappear completely anytime soon. 
* Passenger travel information — The real-time locations of transit vehicles and their expected arrival/ departure times are made available to users via: digital message boards at transit stops, smartphone apps, SMS, and on the company website. • Road obstacle and accident alerts — Will be displayed on the dynamic message signs above highways/freeways. They are broadcast to vehicles which have Traffic Message Channel (TMC) enabled. In the future, obstacle and accident alerts will be broadcast via V2V and V2I channels. 
* Telematics and eCall — Telematics services provide the driver with information about the route, traffic congestion, road obstacles, accident alerts, roadside assistance, and eCall. eCall can connect the vehicle to roadside assistance or with emergency services. eCalls to emergency services can be done manually or automatically if the vehicle detects it is in an accident. 
* Emergency vehicle warning systems — In the future, emergency vehicles will be able to send a voice warning to the FM radio receiver of the car in front advising them to move aside.45 Additionally, V2V/V2I messages will audibly and visibly warn drivers to move aside for emergency vehicles. 
* Road information displays and alert systems — Are above roadway gantry mounted electronic traffic signs for displaying important messages to travelers. These signs are used for displaying messages about traffic congestion, accidents or incidents, road works, speed limits, wait times, lane signals, etc. 
* Communication cell towers, antennas, and repeaters — These are the backbone hardware for ITS communications. There is a shared responsibility between the telco and ITS providers for the installation, upkeep, and maintenance of the communication hardware. 
* I2I, V2V, and V2I communications — In the future, all connected vehicles will be mandated to communicate, in an ad-hoc manner, with other connected vehicles and smart road infrastructure, providing them information such as: location data, safety warnings, and surrounding traffic information. Communications will be done using wireless technology such as: 3G, 4G/LTE, 5G, 802.11g/n/p, 802.16, etc.



