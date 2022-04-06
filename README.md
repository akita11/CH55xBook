# 「PICやAVRの代わりにCH55xはどうでしょう」サポートページ

書籍「PICやAVRの代わりにCH55xはどうでしょう」の更新履歴や追記情報、サポート情報などをまとめていきます。

- 電子書籍版: [技術書典マーケット](
https://techbookfest.org/product/5803512929714176?productVariantID=6092886267396096)
- 冊子版: [スイッチサイエンスのマーケットプレイス](https://www.switch-science.com/catalog/7927/)

## ver1.0 (2022/1/22)

- 初版

## ver1.1 (2022/1/29)

- CH558/9のLEDCtrlについて追記（NeoPixel互換ではない）
- SDCCでのxRAM区画のレジスタの指定ではSFRXを使う
- IOピンのプルアップ抵抗がリセット時にON
- CH559のブートロード方法（P4.6=0として電源ON）
- [KiCADライブラリ](https://github.com/akita11/KiCAD_Library_CH55x)
- 内蔵レギュレータの3.3V出力の電流（100mA程度までは使えそう）
- 4種類のボードの写真: [CH559Pico](https://github.com/akita11/CH559Pico) / [CH552Xiao2](https://github.com/akita11/CH552Xiao2)/ [CH552duino](https://github.com/akita11/CH552duino) / [ProMicroCH552](https://github.com/akita11/ProMicroCH552)

## 次の更新版に追記する予定の情報

- M1 MacでのArduinoIDEの書き込みで、書き込みツールの置き換えをしなくても動作OKの情報あり
- IO電圧の範囲。CH551/2は基本5V、USB信号がつながるピン（P3.6/7）は3.3Vレベルのみ、ほかは5V。CH558/9は基本3.3V、P1.0-7とP4.6/7のみ5V入力OK
- (p.5)NT鯖江の日付（2022年11月27日→2021年11月27日）
- (2.2節）内蔵オシレータの精度（キャリブレーションできない）はUSBペリフェラルには十分だがUSBホストには不十分で外付けオシレータが必要。
- (2.2節）IOピンのプルアップ抵抗は70kΩ（とQuasi-bidirectionalモードのプルアップ用の10kΩ）
- (2.2節後半、v1.1での追記分）「CH55xではプルダウン抵抗が」→「CH55xではプルアップ抵抗が」
- LEDCtrlは、一般的なLEDパネル制御用との情報あり
- 内蔵フラッシュは1000回程度の書き換えでも、（少なくとも短期間の保持性能は）問題ないとの情報あり
- POR (PowerOnReset)回路にクセがある。RST>VIH後5ms程度リセット保持→解除
- BOD (Brown Out Detect)回路がないので、電源電圧が変動しやすいときは注意。特にVDD=2V付近で中途半端にリセット解除（起動）してハング（暴走）することがある。
- WCH純正書き込みツール（WCHISPtool）を使うとき、デバイス一覧に出てこないときは、ドライバをlibusbからWCHドライバ（CH375_A64ドライバ）に戻す（デバイスマネージャから削除→挿し直し）

# Author

Junichi Akita (@akit11, akita@ifdl.jp)
