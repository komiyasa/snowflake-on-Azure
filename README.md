# Snowflake を Azure Marketplace 経由で導入する — お客様向けご案内

本資料は、Azure Marketplace を通じて Snowflake を調達する際の主な利点や検討ポイントを、経営層・調達部門・IT 部門のお客様向けにわかりやすくまとめた説明資料です。コスト、調達、ガバナンス、運用、技術連携の観点から導入時のポイントを整理しています。

---

## 要点（TL;DR）

- 未消化の MACC（Azure Consumption Commitment）を Snowflake の利用料で 100% 消化できます。
- 請求・契約を Microsoft に一本化することで、調達・経理フローを簡素化できます。
- EA のボリューム割引と Snowflake の Private Offer を組み合わせてコスト最適化が可能です。
- Azure AD、Private Link、Key Vault などの Azure ネイティブ機能とシームレスに連携し、既存のガバナンスを継承できます。
- Fabric、Synapse、Power BI、Azure OpenAI などと同じプラットフォーム上でデータ利活用を拡張できます。

---

## 購入パターン（概要）

| パターン | 支払モデル | MACC カウント | 推奨シーン |
| :--- | :--- | :---: | :--- |
| Marketplace 従量課金 (PAYG) | 使った分だけ毎月課金 | **100 %** | スモールスタート／PoC に適しています |
| Marketplace Private Offer | 1–3 年分を前払いコミット | **100 %** | 本番導入で単価最適化を図る際に推奨 |
| Snowflake 直接契約 | Snowflake に直接請求 | 0 % | 既存の直接契約を継続する場合 |

注：MACC に充当できるのは「Azure benefit eligible」と表示される SKU のみです。クレジットカード決済や AppSource、Snowflake 直接契約は対象外となる場合があります。

---

## コスト・調達面のメリット

- **MACC の有効活用**：未消化のコミット残高に Snowflake 利用料を充当することで、予算を有効に活用できます。
- **請求・契約の一本化**：Azure の月次請求に組み込むことで請求業務が簡素化され、ベンダー管理も統合できます。
- **割引の組み合わせ**：EA のボリューム割引と Snowflake の Private Offer を組み合わせることで、より有利な単価を実現できます。
- **調達スピード**：Marketplace 標準契約を利用すれば、社内の発注フローを速やかに進められる場合があります。

---

## ガバナンス・運用面のメリット

- **ID・アクセス管理の継承**：Azure AD（Entra ID）による SSO を利用でき、既存の認証・アクセス制御（MFA、条件付きアクセスなど）を継承できます。
- **ネットワーク分離**：Azure Private Link によってトラフィックを Microsoft のバックボーン内に留めることができ、セキュリティ要件への適合が容易です。
- **コスト可視化**：Azure Cost Management や Power BI を用いて、Snowflake の利用状況を組織内で可視化できます。

---

## 技術的な拡張性

- **Azure エコシステムとの親和性**：Fabric、Synapse、Power BI、Azure OpenAI Service 等と連携し、分析・AI の活用を段階的に拡大できます。
- **SLA とサポート**：Marketplace での調達であっても、Snowflake の標準的な SLA・サポートは維持されます。
- **将来の AI/分析シナリオ**：RAG（Retrieval-Augmented Generation）や Copilot、Agent といった生成AI のユースケース構築がしやすくなります。

---

## 導入の流れ（概略：PAYG の例）

1. Azure ポータルにログインし、「リソースの作成」→「SaaS」で "Snowflake" を検索します。
2. フィルタで "Azure benefit eligible only" を有効にし、対象のプランとリージョンを選択してサブスクライブします。
3. 数分で接続情報（URL 等）が発行されます。発行後は Azure AD SSO、ストレージ連携（Storage Integration）、Private Link 等の設定を行います。
4. 本番導入時は Private Offer の検討や契約条件の調整を Snowflake 側の営業担当と行ってください。

推奨：調達部門と IT 部門で事前に「MACC の残高・用途」「社内請求フロー」「必要なセキュリティ制約（Private Link／Key Vault 等）」を確認しておくと導入が円滑に進みます。

---

## よくあるご質問（FAQ）

Q. Marketplace 経由で購入すると MACC に確実に充当されますか？  
A. 「Azure benefit eligible」と表示される SKU の場合、MACC に充当されます。購入前に SKU 表示をご確認ください。

Q. サポート窓口はどちらになりますか？  
A. 請求・契約は Microsoft 経由になりますが、技術的なサポートや Snowflake 製品に関する SLA は Snowflake の標準サポートが適用されます。詳細は契約条件をご確認ください。

Q. 既存の Snowflake 直接契約がある場合はどうすればよいですか？  
A. 既存契約の状況と比較し、コストやガバナンス要件を考慮して Marketplace への切替（もしくは混在運用）を検討します。調達部門・法務・営業担当と連携してください。

---

## 参考リンク

- Snowflake – Azure Marketplace  
  <https://azuremarketplace.microsoft.com/ja-jp/marketplace/apps/snowflake.snowflake_contact_me>

- Azure Consumption Commitment Benefit (MACC)  
  <https://learn.microsoft.com/ja-jp/azure/marketplace/azure-consumption-commitment-benefit>

- Snowflake Federated Authentication (Azure AD SSO)  
  <https://docs.snowflake.com/en/user-guide/admin-security-fed-auth-overview>

- Snowflake on Azure Private Link  
  <https://docs.snowflake.com/en/user-guide/privatelink-azure>

---

ご不明点やお客様固有の要件がある場合は、調達担当者・ご担当部門とご相談のうえ、個別にご案内いたします。
