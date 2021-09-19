<template>
  <div>
    <h3>フォーム関連の要素</h3>
<pre>
1-10-1 form要素

1-10-2 input要素
type属性

1-10-3 textarea要素

1-10-4 button要素

1-10-5 select要素

1-10-6 option要素

1-10-7 optaroup要素

1-10-8 meter要素

<p>ディスク使用量：
<meter min="0" max="300000000" value="230000000">
容量：300,000,000 バイト<br>
使用領域：230,000,000 バイト
</meter>
</p>

1-10-9 progress要素

<p>処理の進行状況：
<progress id="pbar" value="0" max="100"><span>0</span>%</progress>
</p>

1-10-10 datalist要素

<p>
    <label>
        取得したい資格：
        <input type="text" name="c" list="certifications">
        <datalist id="certifications">
            <option value="HTML5プロフェッショナル認定試験" />
            <option value="ウェブデザイン技能検定" />
            ・・・
        </datalist>
    </label>
</p>

<p>
    <label>
        取得したい資格：
        <input type="text" name="c1" list="certifications">
    </label>
    <datalist id="certifications">
        <br>
        <label>
            ※上の入力欄に入力するか、次のメニューから選択してください：
            <br>
            <select name="c2">
                <option value="">（未選択）</option>
                <option>HTML5プロフェッショナル認定試験</option>
                <option>ウェブデザイン技能検定</option>
            </select>
        </label>
    </datalist>
</p>

1-10-11 output要素

<form onsubmit="return false" oninput="sum.value=a.valueAsNumber+b.valueAsNumber">
    <input name="a" type="number"> +
    <input name="b" type="number"> =
    <output for="a b" name="sum"></output>
</form>

1-10-12 keygen要素

<form action="keysample.cgi" method="post">
    <p><keygen name="pubkey"></p>
    ・・・
    <p><input type="submit" value="送信"></p>
</form>

1-10-13 label要素

<label><input type="checkbox" name="agree"> 同意する</label>

<input type="checkbox" name="agree" id="ag">
<label for="ag">同意する</label>

1-10-14 fieldset要素

1-10-15 legend要素

<fieldset>
    <legend>個人情報</legend>
    <p>
        <label>
            名前：<br>
            <input type="text" name="nm">
        </label>
    </p>
    <p>
        <label>
            住所：<br>
            <textarea name="ad" rows="3"></textarea>
        </label>
    </p>
</fieldset>

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
