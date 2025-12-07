# Type 25 Radio Simulator (二五式空一号無線機シミュレータ)

架空の日本海軍無線機「二五式空一号無線機」を再現したブラウザベースのシミュレーターです。
Web Audio APIによるリアルタイム音声合成と、Canvasによるソナー/オシロスコープのビジュアライゼーションを特徴としています。


## 機能 (Features)

*   **アナログ音声合成**: 800Hzの正弦波、バックグラウンドノイズ、物理的な打鍵音（クリック音）をリアルタイム生成。
*   **イコライザー (EQ)**: 10バンドEQにより、通信環境（ノイズ量、信号の太さ、低音の唸り）を調整可能。
*   **ビジュアル**:
    *   **Sonar (Waterfall)**: 信号履歴をスペクトログラム風に表示。
    *   **Oscilloscope**: リアルタイム波形モニタ。
    *   **CRT Effect**: 走査線と周辺減光によるブラウン管モニタの再現。
*   **操作**:
    *   **手動打鍵**: スペースキーまたは画面タップでモールス信号を送信。
    *   **自動送信**: 史実の信号（トラトラトラ、ニイタカヤマノボレ）を自動再生。
    *   **デコーダー**: 打った信号をリアルタイムで文字変換し、ログに表示。

## 使い方 (Usage)

1.  **起動**: 画面をクリックしてシステムを初期化してください（音声再生のため必須）。
2.  **打鍵**:
    *   PC: [Space] キー、または画面の何もない場所をクリック。
    *   スマホ: 画面の何もない場所をタップ。
3.  **タブ切り替え**:
    *   `AUDIO`: イコライザー設定画面。
    *   `DEC/SCOPE`: ソナーと波形モニタ画面。
4.  **ボタン**:
    *   `TORA / 1208`: 自動再生。
    *   `CLICK`: 打鍵音（カシャカシャ音）のON/OFF。
    *   `TRANS`: 透過モード（背景を透明化）の切り替え。

## 動作環境 (Compatibility)

*   **PC**: Google Chrome, Edge, Firefox, Safari (最新版推奨)
*   **Mobile**: iOS Safari, Android Chrome (横画面推奨)

## 免責事項 (Disclaimer)

1.  **大音量注意**: 本シミュレーターはノイズ音や高周波音（800Hz）を使用します。ヘッドホンをご使用の際は音量にご注意ください。
2.  **点滅注意**: 画面上のランプやインターフェースが激しく点滅する場合があります。光過敏性発作等のリスクがある方はご注意ください。
3.  **無保証**: 本ソフトウェアの使用により生じた損害について、作者は一切の責任を負いません。
4.  **フィクション**: 本ツールに登場する無線機「二五式空一号無線機」は架空の存在です。実際の無線機の挙動やモールス符号の完全な正確性を保証するものではありません。

## クレジット (Credits)

本プロジェクトのコアロジックおよびコード実装は、AIアシスタントによって生成されました。

*   **Code Generation**: Google Gemini 3
*   **Concept & Direction**: [EndoKarasuno]

## ライセンス (License)

MIT License

Copyright (c) 2025 [EndoKarasuno]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.