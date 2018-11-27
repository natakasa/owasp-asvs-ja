# V15: ビジネスロジック検証要件

## 管理目標

検証されるアプリケーションが以下の上位レベルの要件を満たしていることを確認します。

* ビジネスロジックフローはシーケンシャルであり、迂回できず、順番に処理されます。
* ビジネスロジックには継続的な小額の資金転送や一度に百万の友人の追加などの自動攻撃を検出および防御するための制限を含んでいます。
* 高価値のビジネスロジックフローでは悪用ケースや悪意のある人物を考慮し、なりすまし、改竄、否認、情報漏洩、権限昇格の攻撃に対する保護を有しています。

## セキュリティ検証要件

| # | 説明 | L1 | L2 | L3 | 導入バージョン |
| --- | --- | --- | --- | -- | -- |
| **15.1** | アプリケーションはシーケンシャルにビジネスロジックフローのみを処理し、すべての手順は現実的な人的時間で処理され、順序のずれ、スキップされた手順、他のユーザーからの手順、サブミットが速過ぎるトランザクションを処理しないことを検証します。 |  | ✓ | ✓ | 2.0 |
| **15.2** | アプリケーションはビジネス上の制限があり、ユーザー単位に適切に実施しており、自動化された攻撃や異常な攻撃に対して構成可能なアラートや自動応答を行えることを検証します。 |  | ✓ | ✓ | 2.0 |

## 参考情報

詳細については、以下も参照してください。

* [OWASP Testing Guide 4.0: Business Logic Testing](https://www.owasp.org/index.php/Testing_for_business_logic)
* [OWASP Cheat Sheet](https://www.owasp.org/index.php/Business_Logic_Security_Cheat_Sheet)