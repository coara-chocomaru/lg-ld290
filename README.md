# RKDevTool を使った基本的な書き込み手順（lg-ld290）

## 📦 事前準備

以下のファイルを用意してください。

- 下記releaseページから`lg_data.zip`をダウンロードします。
- [lg_data.zip](https://github.com/coara-chocomaru/lg-ld290/releases/download/ld290/lg_data.zip)
- Windows PC
- lg-ld290
- 端末専用の電源ケーブル
- MicroUSB type-b ケーブル（データ通信可能なもの）
---

## ① lg_data.zip を展開

まず最初に **`lg_data.zip`** を任意のフォルダに展開します。

```text
例：C:\Users\YourName\Desktop\lg_data\
```

---

## ② USB ドライバーのインストール

展開したフォルダ内にある以下のパスを開きます。

```text
lg_data\driver\Driverinstall.exe
```

### 手順

1. `Driverinstall.exe` を **ダブルクリック**
2. 画面の指示に従ってインストール
3. インストール完了まで待機

> ⚠️ **注意**  
> Windows のセキュリティ警告が出た場合は、内容を確認した上で許可してください。

---

## ③ RKDevTOOL を起動

ドライバーのインストールが完了したら、以下のファイルを起動します。

```text
lg_data\RKDevTOOL.exe
```

### 起動後の画面例

![RKDevTOOL 起動画面](https://raw.githubusercontent.com/coara-chocomaru/lg-ld290/refs/heads/main/00.jpg)

---

## ④ 端末（lg-ld290）を接続

次に **lg-ld290** を PC に USB 接続します。

### 手順

1. USB ケーブルで **lg-ld290 ↔ PC** を接続してから
2. ld290の **電源を入れ直す**

### 正常に認識された場合

RKDevTOOL 左下に以下の表示が出ます。

```text
Found One LOADER Device
```

#### 表示例

![LOADER 認識](https://raw.githubusercontent.com/coara-chocomaru/lg-ld290/refs/heads/main/_20260207_185956.JPG)

---

## ⑤ 書き込み設定

### Partition 設定画面

![Partition 設定画面](https://raw.githubusercontent.com/coara-chocomaru/lg-ld290/refs/heads/main/01.jpg)

### 設定内容

1. **Partition リスト** から
 - 書き込みたいパーティションにチェック✔
2. **Write by Address** にもチェック✔

---

## ⑥ 書き込み開始

設定が完了したら、左下側の **Run** ボタンを押します。

```text
▶ Run
```

書き込み処理が自動で開始されます。

---

## ⑦ 書き込み完了

処理が正常に完了すると、以下の表示が出ます。

```text
Download image OK
```

### 完了画面例

![Download image OK](https://raw.githubusercontent.com/coara-chocomaru/lg-ld290/refs/heads/main/02.jpg)

---

## ⑧ 書き込み完了後

1. 自動でrebootして再認識されます
   ```text
   Found One LOADER Device
   ```
   と左下に表示されたら
2. **PCからUSB ケーブルを抜く**
3. 端末の **電源ケーブルを挿し直す**

これで起動したら作業は完了です✌️

---

## ❗ トラブルシューティング

### 端末を認識しない場合

以下を試してください。

- USB ドライバーの再インストール
- USB ポートを変更
- USB ケーブルを変更
- PC を再起動
- 端末の電源ケーブルを挿し直す

> 🙇 **環境差が大きいため、ドライバー周りは試行錯誤が必要な場合があります**

---
