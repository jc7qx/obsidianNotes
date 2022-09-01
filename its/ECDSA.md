ECDSA用於訊息交換的簽章與驗證，以確保交換資料的完整性、真實性、及non-repudiation。ETSI TC ITS建議使用 ecdsa_nistp256_with_sha256 公共金鑰，當然也可採用其他金鑰的彈性。

訊息簽章的流程步驟
* 使用雜湊函數（例如，SHA-256）對要保護的訊息純文字計算訊息摘要。例如，要簽章CAM訊息，針對CAM的protocol_version, header_fields, payload_field, 以及 trailer_fields的長度與 trailer field的簽章類型進行計算摘要。
* 將訊息摘要以公鑰演算法（如ecdsa_nistp256_with_sha256）及ITS傳送的私鑰予以加密，產生訊息簽章。
* 根據原始訊息文字、計算而得得簽章、及ITS傳送的認證建立數位簽章訊息

值得注意，依據ETSI ITS的安全描述，ITS傳送的認證可能不會包含在每一個簽證的訊息中。例如，僅一定時間內類型認證的元件包含在被簽證的CAM中，或當request_unrecognized_certificate由附近的ITS站台收到。主要目的希望減少訊息負荷及改善 ITS 通訊的擴展性。

![[Pasted image 20220901123702.png]]

當ITS站台接受到簽證的訊息後，訊息驗證步驟如下
* 由 SecuredMessage 取出訊息文字，經由雜湊函數計算訊息摘要。
* 由 SecuredMessage 取出訊息簽章，並使用公鑰與私鑰解密，產生訊息摘要。
* 接收者比較解密後的訊息摘要及新計算出的訊息摘要，如果二個摘要相同，表示訊息有效，收到的訊息具備完整性及身份驗證性。
值得注意，依據ETSI ITS的安全描述，SecuredMessage的內容可能檢查安全描述的的規則。例如，

![[Pasted image 20220901123754.png]]
