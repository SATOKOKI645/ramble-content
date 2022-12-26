<!-- wp:paragraph -->
<p>これはアドベントカレンダーの16日目(遅刻)の記事です。<br><a rel="noreferrer noopener" target="_blank" href="https://adventar.org/calendars/7404">https://adventar.org/calendars/7404</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>fishは大変良いものでしたが、思ったよりもfish特有の設定方法やGUIのconfigシステムが煩わしく、少し設定が煩雑でした。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>特に、環境変数の設定などで"fish_add_path"コマンドを要求される時に、「あれ、詳細な構文ってなんだっけ」と調べる時間が若干ストレスでした。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>そこで、いっそzshに乗り換えてしまおうかと思ったのでやってみます。</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>zsh-autosuggestionsを使う</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>ターミナルのコマンド履歴を参照して候補を表示、入力補完もするという</strong>とても便利なプラグインです。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>個人的には、コマンドをいちいち打つことで反復の効果はあると思いますが、一定数を超えるとストレスになって来ました。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>面倒くさがりなので、fishの標準機能であったサジェスト機能は是非欲しいと思うようになりました。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>やり方は<a href="https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md" target="_blank" rel="noreferrer noopener">公式のインストールガイド</a>の通りです。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>・Antigen<br>・パッケージ<br>・gitクローン<br>・Oh My Zsh</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>がありますが、今回はgitクローンで入れます。そのほかの方法でも変わりないです。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><em>※ Mac, Alacrittyの環境で行いました</em></p>
<!-- /wp:paragraph -->

<!-- wp:embed {"url":"https://github.com/zsh-users/zsh-autosuggestions"} -->
<figure class="wp-block-embed"><div class="wp-block-embed__wrapper">
https://github.com/zsh-users/zsh-autosuggestions
</div></figure>
<!-- /wp:embed -->

<!-- wp:heading -->
<h2>インストール</h2>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li>このリポジトリを、どこかにクローンしてください。<br>今回は <code>~/.zsh/zsh-autosuggestions</code> にしました。</li><li>下記のコマンドを実行します。<br>クローン先が違う場合は、一部改変してください。<br><code>git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions</code></li><li>設定の反映のために、以下をコマンドで実行します。<br><code>source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh</code></li><li>ターミナルを再起動します。</li></ol>
<!-- /wp:list -->

<!-- wp:heading -->
<h2>全部できたらこんな感じ！</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>そうしたら下記のような感じで、サジェスト機能が利用できます！</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":2748,"width":838,"height":472,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large is-resized"><img src="https://ramble.impl.co.jp/wp-content/uploads/2022/12/スクリーンショット-2022-12-20-0.29.41-510x287.png" alt="" class="wp-image-2748" width="838" height="472"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>コマンド候補が表示されたときキーボードの<code>→</code>キー、もしくは<code>End</code>キーを押したら自動補完できます。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>めちゃくちゃ便利！</p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:paragraph -->
<p>zsh-completionsという拡張機能もあるみたいなので、どちらでもお好きな方をお選びください。</p>
<!-- /wp:paragraph -->