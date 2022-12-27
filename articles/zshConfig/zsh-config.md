これはアドベントカレンダーの16日目(遅刻)の記事です。
https://adventar.org/calendars/7404

fishは大変良いものでしたが、思ったよりもfish特有の設定方法やGUIのconfigシステムが煩わしく、少し設定が煩雑でした。

特に、環境変数の設定などで”fish_add_path”コマンドを要求される時に、「あれ、詳細な構文ってなんだっけ」と調べる時間が若干ストレスでした。

そこで、いっそzshに乗り換えてしまおうかと思ったのでやってみます。

## zsh-autosuggestionsを使う
ターミナルのコマンド履歴を参照して候補を表示、入力補完もするというとても便利なプラグインです。

個人的には、コマンドをいちいち打つことで反復の効果はあると思いますが、一定数を超えるとストレスになって来ました。

面倒くさがりなので、fishの標準機能であったサジェスト機能は是非欲しいと思うようになりました。

やり方は公式のインストールガイドの通りです。

・Antigen
・パッケージ
・gitクローン
・Oh My Zsh

がありますが、今回はgitクローンで入れます。そのほかの方法でも変わりないです。

※ Mac, Alacrittyの環境で行いました


GitHub - zsh-users/zsh-autosuggestions: Fish-like autosuggestions for zsh
Fish-like autosuggestions for zsh. Contribute to zsh-users/zsh-autosuggestions development by creating an account on GitHub.

github.com
## インストール
このリポジトリを、どこかにクローンしてください。
今回は ~/.zsh/zsh-autosuggestions にしました。
下記のコマンドを実行します。
クローン先が違う場合は、一部改変してください。
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
設定の反映のために、以下をコマンドで実行します。
source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh
ターミナルを再起動します。
## 全部できたらこんな感じ！
そうしたら下記のような感じで、サジェスト機能が利用できます！


コマンド候補が表示されたときキーボードの→キー、もしくはEndキーを押したら自動補完できます。

めちゃくちゃ便利！

zsh-completionsという拡張機能もあるみたいなので、どちらでもお好きな方をお選びください。