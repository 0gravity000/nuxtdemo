<template>
  <div>
    <h3>セクションと基本構造</h3>
<pre>
1-5-1 セクションと見出しの関係

<!DOCTYPE html>
<html lang="ja">
<head>
    <title> ・・・ </title>
</head>
<body>
    <h1>見出しA</h1>
    <h2>見出しB</h2>
    <blockquote>
        <h3>見出しC</h3>
    </blockquote>
    <h2>見出しD</h2>
    <section>
        <h3>見出しE</h3>
    </section>
</body>
</html>

<header>
    <h1>見出し</h1>
    <p>サブタイトル</p>
</header>

1-5-2 h1～h6要素

<header>
    <h1>合格への道 III</h1>
    <p>そして面接へ…</p>
</header>

1-5-3 article要素

<article>
    <header>
        <h1>レベル1認定試験に合格しました！</h1>
        <p><time>2017-04-01 22:18:05</time></p>
    </header>
    <p>先日、夢の中にセマンくんが出てきたんです。</p>
    <p>そしてガラガラのヘンな声で、私にこう言ったんです。</p>
    <p>「全身の70%以上をオレンジ色にして受験したら合格するがね！」</p>
    ・・・
    <section>
        <h2>コメント</h2>
        ・・・
    </section>
</article>

1-5-4 section要素

<body>
    <h1>合格のための心得</h1>
    <section>
        <h2>その1：本書を購入する</h2>
        <p>これを読んでいるあなたはきっと大丈夫です。</p>
        <p>選択のセンスがありますので、五択問題も心配無用！</p>
    </section>
    <section>
        <h2>その2：最後まで読む</h2>
        <p>本書の内容はおおむね重要な順になっています。</p>
        <p>とにかく読めるところまで読んでおくと合格に近づけます！</p>
    </section>
</body>

1-5-5 aside要素

<aside>
    <h3>広告</h3>
    <a href="http://html5exam.jp/">
        <section>
            <h4>HTML5プロフェッショナル認定試験</h4>
            <p>取得したい資格No.1</p>
            <p>多くの企業が推進する次世代Web言語の認定資格</p>
        </section>
    </a>
    <a href="https://book.mynavi.jp/">
        <section>
            <h4>マイナビBOOKS</h4>
            <p>よくわかる教科書シリーズ</p>
            <p>好評発売中！</p>
        </section>
    </a>
</aside>

1-5-6 nav要素

<body>

<header>
    <h1>株式会社◯◯◯</h1>
    <ul>
        <li><a href="#">サイトマップ</a></li>
        <li><a href="#">Global</a></li>
    </ul>
    <nav>
        <ul>
            <li><a href="#">ホーム</a></li>
            <li><a href="#">お知らせ</a></li>
            <li><a href="#">製品情報</a></li>
            <li><a href="#">会社概要</a></li>
            <li><a href="#">お問い合わせ</a></li>
        </ul>
    </nav>
</header>

<main>
    ～ メインコンテンツ ～
</main>

<footer>
    <ul>
        <li><a href="#">プライバシーポリシー</a></li>
        <li><a href="#">利用規約</a></li>
    </ul>
    <p>
        <small>Copyright &copy; 2017 ◯◯◯. All rights reserved.</small>
    </p>
</footer>

</body>

1-5-7 header要素

<body>
<header>
    <h1>株式会社◯◯◯</h1>
    <nav>
        <ul>
            <li><a href="#">ホーム</a></li>
            <li><a href="#">お知らせ</a></li>
            <li><a href="#">製品情報</a></li>
            <li><a href="#">会社概要</a></li>
            <li><a href="#">お問い合わせ</a></li>
        </ul>
    </nav>
</header>
・・・

1-5-8 footer要素

・・・
<footer>
    <ul>
        <li><a href="#">プライバシーポリシー</a></li>
        <li><a href="#">利用規約</a></li>
    </ul>
    <p>
        <small>Copyright &copy; 2017 ◯◯◯. All rights reserved.</small>
    </p>
</footer>
</body>

<article>
    <footer><a href="#">前ページ</a></footer>
    <h1>レベル1認定試験に合格しました！</h1>
    <p>本日は、ブログでちょっとだけ自慢しちゃいますよ。</p>
    <p> ・・・ </p>
    <footer><a href="#">前ページ</a></footer>
</article>

1-5-9 main要素

<body>

<header>
    <h1>◯◯◯スクール</h1>
    <nav>
        <ul>
            <li><a href="#">ホーム</a></li>
            <li><a href="#">コース紹介</a></li>
            <li><a href="#">会社概要</a></li>
            <li><a href="#">お問い合わせ</a></li>
        </ul>
    </nav>
</header>

<main>
    <article>
        <header>
            <h1>会社概要</h1>
            <p>日本でトップクラスの合格実績！</p>
        </header>
        <section>
            <h2>合格率100%！（当社調べ）</h2>
            <p>嘘だと思ったら食べてください。</p>
        </section>
        ・・・
    </article>
</main>

<footer>
    <p>
        <small>Copyright &copy; 2017 ◯◯◯. All rights reserved.</small>
    </p>
</footer>

</body>

1-5-10 address要素

<footer>
  <address>
    お問い合わせは下記メールアドレスまでお願いします。<br>
    <a href="mailto:info@example.com">info@example.com</a>
  </address>
  <p>
    <small>Copyright &copy; 2017 ◯◯◯. All rights reserved.</small>
  </p>
</footer>

1-5-11 div要素

1-5-12 span要素

<h1>
    合格への道<br>
    <span class="subtitle">こうして僕は三日でおぼえた！</span>
</h1>

</pre>
  </div>
</template>

<script>
export default {
  layout: 'LayoutHtmlcss',
  data () {
    return {
    }
  }
}
</script>

<style scoped>
</style>
