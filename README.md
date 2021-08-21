# Name

kana-display

# Note

プログラムの改変, 再配布はご自由です。  
再配布の場合は, Readmeなどにその旨を書いてくれると嬉しいです。

[English]  
This is a program for Japanese. After that, it will be written in Japanese and English using Google Translate.  
You are free to modify or redistribute the program.  
In the case of redistribution, I would be grateful if you could write that fact in the Readme etc.

# Usage

追加されるブロックは表示ブロックと数値を文字列に変換するブロックの2つです。  
表示ブロックは、本来表示できないひらがな／カタカナ／一部記号の表示ができます。また、普通の英数字（半角/全角対応）も表示可能です。  
数値を出力したい場合は, 数値を文字列に変換するブロックを使うと表示することが可能です。
 
スラッシュ(/と／), バックスラッシュ(\と＼)は半角/全角でフォントが異なりますが, 他は半角/全角によるフォントの差異はありません。  
 ※半角のバックスラッシュ(\)は, \\のように2つ入力する必要があります。(例: \(^o^)/を表示する場合 => \\(^o^)/)
 
第4因数まで設定できます。  
 第1引数 => 表示文字列(必須)  
 第2引数 => 表示のスクロール速度(デフォルト: 100ms)  
 第3引数 => 表示が消えるまでスクロールするか(デフォルト: true)  
 第4引数 => コンソールにログの出力をするか(デフォルト: false, ブロックでは設定不可)  
ex.print(data: string, scroll_speed: number = 100, disp_off: boolean = true, console_output: boolean = false): void
 
また, 表示文字列に数値は設定出来ないので, 変数などから数値を表示したい場合は, 数値→文字列に変換するブロックを使って下さい。  
もしくは, 数値 + ""のようにすると文字列に変換してくれます。  
× ex.print(123);  
◯ ex.print(tostring(123));  
◯ ex.print(123 + "");  
 
[English]  
There are two blocks to be added: a display block and a block that converts numbers to strings.  
The display block can display hiragana / katakana / some symbols that cannot be displayed originally. In addition, ordinary alphanumeric characters (half-width / full-width compatible) can also be displayed.  
If you want to output a numerical value, you can display it by using a block that converts the numerical value to a character string.  
 
The fonts for slashes (/ and ／) and backslashes (\ and ＼) are different for half-width / full-width characters, but there is no difference in fonts for other characters.  
 * You need to enter two half-width backslashes (\) like \\. (Example: When displaying \(^o^)/ => \\(^o^)/)
 
You can set up to the 4th factor.  
 1st argument => Display string (required)  
 2nd argument => Display scroll speed (default: 100ms)  
 3rd argument => Scroll until the display disappears(default: true)  
 4th argument => Whether to output the log to the console (default: false, cannot be set in the block)  
ex.print(data: string, scroll_speed: number = 100, disp_off: boolean = true, console_output: boolean = false): void
 
Also, since numerical values ​​cannot be set in the display character string, if you want to display numerical values ​​from variables, etc., use a block that converts from numerical values ​​to character strings.
Or, if you use number + "", it will be converted to a character string.  
× ex.print(123);  
◯ ex.print(tostring(123));  
◯ ex.print(123 + "");  
 
 
Translated by Google.

# Author

Asato.



> このページを開く [https://asato65.github.io/kana-display/](https://asato65.github.io/kana-display/)

## 拡張機能として使用

このリポジトリは、MakeCode で **拡張機能** として追加できます。

* [https://makecode.microbit.org/](https://makecode.microbit.org/) を開く
* **新しいプロジェクト** をクリックしてください
* ギアボタンメニューの中にある **拡張機能** をクリックしてください
* **https://github.com/asato65/kana-display** を検索してインポートします。

## このプロジェクトを編集します ![ビルド ステータス バッジ](https://github.com/asato65/kana-display/workflows/MakeCode/badge.svg)

MakeCode でこのリポジトリを編集します。

* [https://makecode.microbit.org/](https://makecode.microbit.org/) を開く
* **読み込む** をクリックし、 **URLから読み込む...** をクリックしてください
* **https://github.com/asato65/kana-display** を貼り付けてインポートをクリックしてください

## ブロックのプレビュー

この画像はマスター内の最後のコミットからのブロックコードを示しています。
このイメージは更新に数分かかる場合があります。

![生成されたブロック](https://github.com/asato65/kana-display/raw/master/.github/makecode/blocks.png)

#### メタデータ (検索、レンダリングに使用)

* for PXT/microbit
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
