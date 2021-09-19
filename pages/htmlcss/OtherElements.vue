<template>
  <div>
    <h3>その他の要素</h3>
<pre>
1-12-1 figure要素

<p>
CSSを使用すると、影を表示させることができます（<a href="#fig01">図版01</a>）。
</p>
<figure id="fig01">
<figcaption>図版01：CSSでボックスに影を表示させる例</figcaption>
<pre><code>.sample {
    box-shadow: 3px 3px 10px #999;
}</code></pre>
</figure>

1-12-2 figcaption要素

<figure>
    <figcaption>札幌の気候</figcaption>
    <img src="temp.png" alt="各月の気温のグラフ：1月の平均気温-3.6℃、2月の ～ ">
    <table border="1">
        <caption>：各月の降水量：単位mm</caption>
        ・・・
    </table>
</figure>

1-12-3 details要素

<hr>
<details>
    <summary>見出し</summary>
    <p>詳細情報</p>
    <p>詳細情報</p>
</details>
<hr>

1-12-4 summary要素

1-12-5 menu要素

<img src="pic.jpg" alt="写真" contextmenu="ctx-menu01">
<menu id="ctx-menu01">
    <menuitem label="項目1" onclick="～" />
    <menuitem label="項目2" onclick="～" />
    <menu label="サブメニュー">
        <menuitem label="サブ項目1" onclick="～" />
        <menuitem label="サブ項目2" onclick="～" />
    </menu>
</menu>

1-12-6 menuitem要素

1-12-7 iframe要素

1-12-8 hr要素

<p>
  「やっぱり、あのオレンジの本を選んでよかったね」と言って知子は微笑んだ。
  僕はもう少し彼女と話していたかったのだが、終電の時間がせまっていたので彼女は先に店を出た。僕にとっては
  二つの意味で喜ばしい夜だった。レベル１を両方ともクリアしたのだ。
</p>
<hr>
<p>
  翌朝、目を覚ますとまぶしいほどの光の筋がカーテンの隙間から部屋に入り込んでいた。
    ・・・
</p>

1-12-9 script要素

1-12-10 noscript要素

1-12-11 template要素

<table border="1">
    <tbody>
        <template id="tb01">
            <tr>
                <td></td><td></td><td></td><td></td>
            </tr>
        </template>
    </tbody>
</table>

1-12-12 canvas要素

<canvas width="800" height="400"></canvas>

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
