# CheckRDP-TCP5985 セットアップ
## 概要
(1) 接続先で、TCP/445, TCP/5985 を開ける。
(2) 接続元で、TrustedHost を登録する。
## 関連コマンド
### 確認
```powershell
(Get-Item WSMan:\localhost\Client\TrustedHosts).Value
```
### 登録
```powershell
Set-Item WSMan:\localhost\Client\TrustedHosts -Value "SV1,SV2" -Force
```
# CheckRDP
(1) 'CheckRDP' for unzip.
(2) Host names separated by commas.
