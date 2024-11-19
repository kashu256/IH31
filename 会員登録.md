```mermaid
sequenceDiagram
    actor 顧客
    actor 担当者
    participant システム
    
    顧客 ->> 担当者: 入会申込書受け取り
    note left of 担当者:入会申込書
    担当者 ->> システム: 会員情報登録
    システム ->> システム:登録処理
    システム ->> 担当者:会員カード発行
    note right of 担当者:会員カード
    担当者 ->> 顧客:会員カード受け渡し
    note left of 担当者:会員カード
```