<template>
  <div>
    <h3>リスト関連の要素</h3>

<pre>
1-7-1 ul要素

<p>沖縄で行ったことのある離島は次の通りです。</p>
<ul>
    <li>ナガンヌ島</li>
    <li>久米島</li>
    <li>竹富島</li>
    <li>黒島</li>
</ul>

1-7-2 ol要素

<p>個人的に沖縄で好きな島は次の通りです（好きな順）。</p>
<ol>
    <li>黒島</li>
    <li>久米島</li>
    <li>ナガンヌ島</li>
</ol>

1-7-3 li要素

<ul>
    <li>黒島</li>
    <li>久米島</li>
    <li>ナガンヌ島</li>
</ul>

1-7-4 dl要素

<dl>
<dt><dfn>HTML5プロフェッショナル認定資格</dfn></dt>
<dd>
HTML5・CSS3・JavaScriptといった最新技術に関する知識をLPI-Japanが中立的な立場で認定する認定資格。
</dd>
</dl>

1-7-5 dt要素

<article>
    <h1>よくあるご質問</h1>
    <dl>
        <dt>どのくらいの正答率で合格できますか？</dt>
        <dd>7割程度の正答率で合格できる設定となっています。</dd>
        <dt>他の資格試験との違いは何ですか？</dt>
        <dd>知識よりも、現場で必要となる能力に重点が置かれています。</dd>
        <dt>回答パターンにはどのようなものがありますか？</dt>
        <dd>「単一選択」「複数選択」「記述式」があります。</dd>
    </dl>
</article>

1-7-6 dd要素

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
