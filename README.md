# ❄️ 大企業向け：Snowflake を **Azure Marketplace** 経由で導入するメリット徹底解説

> **Snowflake を Azure Enterprise Agreement (EA)／Microsoft Azure Consumption Commitment (MACC) 内で調達すると何が変わる？**  
> コスト・ガバナンス・テクニカル統合の 3 つの視点でまとめました。

---

## 📝 TL;DR

- **未消化 MACC** を **Snowflake 利用料 100 %** で一気に消化  
- **請求・契約が Microsoft 一本化** → 調達・経理フローを大幅に簡素化  
- **EA ボリューム割引 × Snowflake Private Offer** で二重ディスカウント  
- **Azure AD／Private Link／Key Vault** とネイティブ統合でガバナンスを継承  
- **Fabric／Synapse／Power BI／OpenAI** と同じ基盤でデータ & AI 活用を爆速拡張  

---

## 1️⃣ 購入パターン早見表

| パターン | 支払モデル | MACC カウント | 代表的シーン |
| :--- | :--- | :---: | :--- |
| **Marketplace 従量課金 (PAYG)** | 使った分だけ毎月課金 | **100 %** | スモールスタート／PoC |
| **Marketplace Private Offer** | 1–3 年分を前払いコミット | **100 %** | 本格導入・単価最適化 |
| **Snowflake 直接契約** | Snowflake に直接請求 | 0 % | 歴史的経緯で継続契約のみ |

> **注意**：「**Azure benefit eligible**」と表示される SKU のみが MACC 消化対象。  
> AppSource のクレジットカード決済や Snowflake 直接契約は対象外です。

---

## 2️⃣ コスト & 調達メリット

| 💰 メリット | 詳細 |
| :--- | :--- |
| **MACC 消化** | Snowflake 利用料がコミット残高を 1 円残らず削る |
| **請求一本化** | Azure 月次請求書に “Marketplace charges > Snowflake” と統合 |
| **Private Offer 割引** | EA ボリューム割引 + Snowflake 容量割引を同時適用 |
| **調達スピード** | Marketplace 標準契約 → PO 発行 → 数時間で環境 Ready |

---

## 3️⃣ ガバナンス & 運用メリット

| 🔒 メリット | 詳細 |
| :--- | :--- |
| **ID 統合** | Azure AD（Entra ID）SSO で MFA／条件付きアクセスを継承 |
| **ネットワーク分離** | Azure Private Link でトラフィックを Microsoft Backbone 内に閉じ込め |
| **コスト可視化** | Azure Cost Management + Power BI でリアルタイム分析 |

---

## 4️⃣ テクニカル拡張メリット

| 🚀 メリット | 詳細 |
| :--- | :--- |
| **Fabric／Synapse／Power BI 連携** | ETL・BI・AI ワークロードを Azure ネイティブで統合 |
| **99.99 % SLA & サポート** | Marketplace 版でも Snowflake 本体の SLA・サポートは維持 |
| **生成 AI への布石** | Azure OpenAI Service と同居 → RAG／Copilot／Agent シナリオ構築が容易 |

---

## 5️⃣ 導入ステップ（PAYG 例）

```bash
# Azure Portal > リソースの作成 > SaaS → "Snowflake" を検索
# フィルタ “Azure benefit eligible only” をオン
# プラン／リージョンを選択して Subscribe
# 数分で URL 発行 → Azure AD SSO & Storage Integration を設定
```

---

## 🔗 参考リンク

- **Snowflake – Azure Marketplace**  
  <https://azuremarketplace.microsoft.com/ja-jp/marketplace/apps/snowflake.snowflake_contact_me>  
  Marketplace 公式リスティング

- **Azure Consumption Commitment Benefit**  
  <https://learn.microsoft.com/ja-jp/azure/marketplace/azure-consumption-commitment-benefit>  
  MACC の概要と適用条件

- **Snowflake Federated Authentication (Azure AD SSO)**  
  <https://docs.snowflake.com/en/user-guide/admin-security-fed-auth-overview>  
  Azure AD 連携ガイド

- **Snowflake on Azure Private Link**  
  <https://docs.snowflake.com/en/user-guide/privatelink-azure>  
  ネットワーク分離のベストプラクティス
