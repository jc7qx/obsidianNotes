協作式與智慧型交通運輸架構參考模型（The Architecture Reference for Cooperative and Intelligent Transportation, ARC-IT）是美國運輸部支持倡導的架構規範，用於規劃、制定、與整合智慧型交通系統。美國與1996年開始發展美國的ITS架構，隨著技術演進及新ITS功能需求，ITS架構演進至目前的ARC-IT。ARC-IT參考架構的開發主要是協助地區建立ITS系統架構，並協助地區政府瞭解如何能夠將地區性的ITS系統納入上層的交通運輸管理架構中。ARC-IT不僅提供ITS系統的共同語言用來描述系統，也提供地區ITS系統建構時的基準元件。為有效描述ITS系統，ARC-IT提出企業（Enterprise）、功能（Functional）、實體（Physical）、與通訊（Communication）等四個觀點，由四個觀點來瞭解ITS的系統架構。
![[Pasted image 20220803170048.png]]


實體觀點（Physical View）
實體觀點描述支持ITS交通運輸各種服務所需的系統及資訊交換。因此，在實體觀體中，ARC-IT提出實體物件（Physical Objects），實體物件間彼此互動與交換資訊以實現ITS的各項服務。實體物件又可細分為二類，一種稱為次系統可以提供ITS功能，另一稱為終端器（Terminators）不提供功能。實體物件間有資訊傳遞以提供ITS服務。實務上，實體物件可以分為「中心」、「現場設備」、「車輛」、「個人裝置」、「支援系統」等。
* 中心：如交通管制中心
* 裝備：如交通號誌控制器
* 車輛：如公車
* 個人裝置：如智慧型手機
* 支援系統：如資料儲存系統、圖資更新系統

ART-IT有49項交通資子系統（如下圖），資系統間有通訊管道提供資訊交換。
![[Pasted image 20220805163626.png]]

* 中心子系統包含「授權中心」、「邊界檢查管理中心」、「商用車輛管理中心」、「商用尺服務提供中心」、「緊急管理中心」、「空氣排放管理中心」、「貨運車隊管理中心」、「貨運運送與後勤中心」、「維修與建築管理中心」、「支付管理中心」、「停車管理中心」、「交通管制中心」、「公共運輸管理中心」、及「運輸資訊中心」。
* 現場設備子系統包含「邊界檢查系統」、「商用車輛檢查設備」、「商用車輛路邊設備」、「電子付費站」、「現場維修設備」、「intermodal terminal」、「ITS道路設施」、「ITS道路支付設備」、「停車場設備」、「路邊通訊單元」、「安全監控設備」、及「旅行支援設備」。
* 車輛子系統包含「商用車輛車載設備」、「緊急車輛車載設備」、「貨運裝置」、「維修與工程車輛車載設備」、「公車車載設備」、「車輛車載設備」。
* 個人裝置包含「個人資訊裝置」、「遠端存取裝置」。
* 支援子系統包含「資料存檔系統」、「認證系統」、「協作式ITS憑證管理系統」、「資料傳送系統」、「識別辨識註冊」、「ITS通訊設備」、「圖資更新系統」、「物件登錄與方線系統」、「服務監督系統」、「支持維護設備」、「廣域資訊傳送器系統」。

以交通訊號控制系統為例，在ARC-IT的架構有２個子系統，分別為交通管理中心(Traffic Management Center)及ITS道路設施。以上二個子系統之間需要有通訊連結以便能交換控制與監控資訊，提供交通號誌控制系統「區域訊號同步」、「幹線網路交通狀況」、及「一系列調控策略」。交通管理中心功能藉由交通管理中的具備的設備來達成，如電腦、交通控制台、視訊交換與顯示系統。ITS道路設備功能藉由道路上的交通號誌控制器與交通燈號、車輛偵測器（如雷達、影像、感應迴路）及攝影機來完成。

ARC-IT總共定義389個功能物件，每一個功能物件包含功能描述及對應的功能需求。以「TMC訊號控制」為例；

>TMC訊號控制提供交通管理員在訊號化的交叉路口監控管理交通車流。須具備分析和減少從交通監控設備收集的資料，及制定和實施信號交叉路口的控制計劃。可以制定和實施控制計劃，在單一交通管理中心的範圍內協調多個交叉路口的信號，並反應交通狀況並適應支持事故、搶占和優先請求、行人過路呼叫等。

TMC訊號控制所對應的功能需求如下：

>01 中心應遠端空制交通號誌控制器
>02 中心應接受行人呼叫的通知
>03 中心應收集交通信號控制器的運行狀態，並與中心發送的控制資訊進行比較。
>04 中心應從現場搜集交通信號控制器故障資料。
>05The center shall manage (define, store andmodify) control plans to coordinate signalized intersections, to be engaged at the direction of center personnel or according toa daily schedule.
>06 The center shall implement control plans to coordinate signalized intersections based on data from sensors.
>07 The center shall manage boundaries of the control sections used within the signal system.
>08 The center shall maintain traffic signal coordination including synchronizing clocks throughout the system.
>09 The center shall implement control plans to coordinate signalized intersections based on data from sensors and connected vehicles.
>10 The center shall adjust signal timing in respond to a signal prioritization, signal preemption, pedestrian call, multi-modal crossing activation, or other requests for right-of-way.
>11 The center shall collect commercial vehicle data (e.g., characteristics, route, schedule) for intermodal freightevents.
>12The center shall adjust signal timing in respond to traffic and environmental parameters at each intersection in real time and adapts sothat the traffic network is optimized using available green time to serve the actual traffic demands while minimizing the environmental impact.
>13 The center shall process collected traffic and environmental data from sensors and connected vehicles.
>14The center shall support requests from emergency management centers to provide responding emergency vehicles with signal preemption. 
>15The center shall monitor, analyze, and store traffic sensor data (speed, volume, occupancy) collected from field elementsat or near signalized intersections.
>16The center shall maintain a database of traffic sensors and associated data (including the roadway on which they are located, the type of data collected, and the ownership of each)
>17The center shall remotely control devices to detect traffic in the vicinity of trafficsignals