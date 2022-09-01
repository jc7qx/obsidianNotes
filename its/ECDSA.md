ECDSA用於訊息交換的簽章與驗證，以確保交換資料的完整性、真實性、及non-repudiation。ETSI TC ITS建議使用 ecdsa_nistp256_with_sha256 公共金鑰，當然也可採用其他金鑰的彈性。

訊息簽章的流程步驟
使用雜湊函數（例如，SHA-256）對要保護的訊息純文字計算訊息摘要。例如，要簽章CAM訊息，針對CAM的protocol_version, header_fields, payload_field, 以及 trailer_fields的長度與 trailer field的簽章類型進行計算摘要。