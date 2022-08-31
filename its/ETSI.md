ETSI ITS是歐洲制定的ITS標準(European Telecommunications Standards Institute, ETSI ITS)，ETSI TS 103 097標準(由IEEE 802.11p修改)定義security headers, certificate format 以及 security profiles，可支持使用橢圓曲線密碼原理(ECC)。

ETSI TC ITS定義存取、網路、及設備等垂直三層安全架構，網路層可以處理地理定位，設備層支援各種應用服務的訊息。層與層之間的安全服務經由特定的服務存取點(Service Access Points, SAP)提供。

![[Pasted image 20220831114440.png]]

### security headers (安全表頭)

ETSI TS 103 097定義各種安全訊息表頭及格式以確保不同的元件的互動，ITS站台間安全資訊交換。主要的安全訊息表頭為「安全訊息結構」定義如何將一般安全訊息編碼，封裝在GeoNetworking封包中。
![[Pasted image 20220831144815.png]]

![[Pasted image 20220831145158.png]]

### Certificate Format

ETSI TS 103 097提出新的驗證格式定義如何針對每一種類型的驗證所需的資訊編碼。
![[Pasted image 20220831145614.png]]

### Security Profiles

ETSI TS 103 097定義CAM, DENM, 一般訊息, 及驗證等四個主要的security profiles，這些security profiles都針對安全演算法（如[[ECDSA]]或[[ECIES/AES]]）支援。