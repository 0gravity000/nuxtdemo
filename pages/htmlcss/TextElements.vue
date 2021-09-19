<template>
  <div>
    <h3>テキスト関連の要素</h3>

<pre>
1-6-1 p要素

1-6-2 a要素
<nav>
  <ul>
    <li> <a href="/">ホーム</a> </li>
    ・・・
  </ul>
</nav>

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

1-6-3 em要素

1-6-4 strong要素

<h1>第1章 <strong>合格への道！</strong></h1>

<p>
<strong>【警告】</strong>
札幌では、たとえ<strong>中央区であっても<strong>ヒグマ</strong>が出没</strong>することがあります。
</p>

1-6-5 blockquote要素

<blockquote>
<p>
メロスは激怒した。必ず、かの邪智暴虐の王を除かなければならぬと決意した。メロスには政治がわからぬ。メロスは、村の牧人である。笛を吹き、羊と遊んで暮して来た。
</p>
<footer>
― <cite>太宰治</cite>（1975） <cite>『走れメロス』</cite>.
</footer>
</blockquote>

1-6-6 q要素

<p>
僕にはぜんぜん記憶がないのだけれど、<cite>ヘルマン・ヘッセ</cite>の<q>そうか、そうか、つまり君はそんな
やつなんだな</q>って意外とみんなおぼえてるみたいですね。
</p>

1-6-7 cite要素

<p>
<cite>水曜どうでしょう</cite>の名セリフと言えば、個人的には<q>ロビンソンもう帰ろうよ</q>だな。
</p>

1-6-8 mark要素

<blockquote>
<p>
<mark>メロスは激怒した。</mark>必ず、かの邪智暴虐の王を除かなければならぬと決意した。メロスには政治がわからぬ。メロスは、村の牧人である。笛を吹き、羊と遊んで暮して来た。
</p>
</blockquote>

<p>
冒頭の文章は、日本人なら誰もが知っている有名な一節です。この文章は・・・
</p>

1-6-9 small要素

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
</html>

1-6-10 data要素

<p>
大藤園より<data value="JAN:4912345678903">こ～い合格茶</data>が発売された。
</p>

1-6-11 time要素

<p>
<time datetime="2017-01-17">昨日</time>の試験はマジで疲れました。
明日は<time>07:30</time>に集合です。
</p>
</html>

1-6-12 abbr要素

<p>
合格したら<abbr title="結婚活動">婚活</abbr>も頑張るぞ！
</p>
</html>

1-6-13 dfn要素

<p>
<dfn>HTML5プロフェッショナル認定資格</dfn>とは、LPI-JapanがHTML5・CSS3・Javascriptなど最新のマークアップに関する技術力と知識を、公平かつ厳正に、中立的な立場で認定する認定資格です。
</p>

1-6-14 b要素

<h1>第3章 <strong>HTML5で変更された要素</strong></h1>
<p>
<b class="lede">新しく追加された要素の次に重要なのは、意味や役割が変更された要素です。本章ではHTML5で変更された要素を重要な順に解説していきます。</b>
</p>

1-6-15 i要素

<p>エゾアカガエルの学名は<i class="taxonomy">Rana pirica</i>です。</p>

1-6-16 s要素

<p>本日限りの大特価！<s>2,800円</s> 980円！</p>

1-6-17 u要素

<p>Hello, <u class="spelling">warld!</u></p>

1-6-18 bdo要素

1-6-19 bdi要素

<ul>
    <li>ユーザー名 <bdi>知子</bdi>: 7 posts.</li>
    <li>ユーザー名 <bdi>ミキティ</bdi>: 10 posts.</li>
    <li>ユーザー名 <bdi> ???? </bdi>: 1 posts.</li>
</ul>
</html>

1-6-20 pre要素

1-6-21 code要素

<p>
HTMLでは、ソースコードは<code>code</code>要素としてマークアップします。
</p>

1-6-22 kbd要素

<p>
次に、<kbd>F3</kbd>キーを押してください。
</p>

1-6-23 samp要素

<pre><samp>
“Macintosh HD”のアクセス権を検証中
アクセス権データベースを読み出しています。
アクセス権データベースの読み出しには数分かかる場合があります。
</samp></pre>

1-6-24 var要素

<p>
CSS3には :nth-child(<var>a</var>n+<var>b</var>) という書式のセレクタがあって、
<var>a</var>と<var>b</var>のところには任意の整数が指定できる。
</p>

1-6-25 sup要素

<p>
<var>E</var>=<var>m</var><var>c</var><sup>2</sup>
</p>

1-6-26 sub要素

<p>
二酸化炭素はCO<sub>2</sub>です。
</p>

1-6-27 br要素

<p>
〒012-3456<br>
北海道札幌市中央区牧志1-2-3<br>
札幌ニフェーデービル7F
</p>

1-6-28 wbr要素

<p>
What does super<wbr>califragilistic<wbr>expiali<wbr>docious mean?
</p>

1-6-29 ins要素

<h1>To Do リスト</h1>
<ul>
    <li>HTML5の本を最後まで読む</li>
    <li><ins>LPI-IDを取得する</ins></li>
    <li><ins>HTML5レベル1試験の受験予約</ins></li>
    <li><ins datetime="2017-12-24">HTML5レベル1試験受験！</ins></li>
</ul>

1-6-30 del要素

<h1>To Do リスト</h1>
<ul>
    <li><del>HTML5の本を最後まで読む</del></li>
    <li><del datetime="2017-04-01T20:30+09:00">LPI-IDを取得する</del></li>
    <li>HTML5レベル1試験の受験予約</li>
    <li>HTML5レベル1試験受験！</li>
</ul>

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
