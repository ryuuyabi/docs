## Cognitoを使用してのOauth2認証方法

### 用語
| 用語 | 概要 |
| --- | --- |
| state | CSRF対策のために導入する |
| code_verifier | RFC7636に準拠する文字列 |
| codeChallenge | code_verifierをハッシュ化してBase64URL形式にエンコードする |

### 処理の流れ
| URL | HTTP | 概要 |
| --- | ---- | --- |
| /oauth/redirect | GET | state・code_verifier・codeChallengeを作成する |
| /oauth/authorize | GET |  |

### フローチャート
