# 「PICやAVRの代わりにCH55xはどうでしょう」サポートページ

書籍「PICやAVRの代わりにCH55xはどうでしょう」の更新履歴や追記情報、サポート情報などをまとめていきます。

## ver1.0 (2022/1/22)

- 初版

## ver1.1 (2022/1/29)

- CH558/9のLEDCtrlについて追記（NeoPixel互換ではない）
- SDCCでのxRAM区画のレジスタの指定ではSFRXを使う
- IOピンのプルアップ抵抗がリセット時にON
- CH559のブートロード方法（P4.6=0として電源ON）
- [KiCADライブラリ](https://github.com/akita11/KiCAD_Library_CH55x)
- 内蔵レギュレータの3.3V出力の電流（100mA程度までは使えそう）
- 4種類のボードの写真: [CH559Pico](https://github.com/akita11/CH559Pico) / [CH552Xiao](https://github.com/akita11/CH552Xiao)/ [CH552duino](https://github.com/akita11/CH552duino) / [ProMicroCH552](https://github.com/akita11/ProMicroCH552)

## 次の更新版に追記する予定の情報

- M1 MacでのArduinoIDEの書き込みで、書き込みツールの置き換えをしなくても動作OKの情報あり
- USB信号がつながるピン（CH552のP3.6/7）は3.3Vレベルのみ。CH558/9についてはデータシートに記載がない

# Author

Junichi Akita (@akit11, akita@ifdl.jp)
