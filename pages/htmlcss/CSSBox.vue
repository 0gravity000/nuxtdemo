<template>
  <div>
    <h3>CSS ボックス</h3>
<pre>
2-8-1 margin 関連プロパティ

2-8-2 padding 関連プロパティ

2-8-3 border 関連プロパティ

2-8-4 幅と高さを設定するプロパティ

2-8-5 boeder-radius プロパティ
ボックスの角を丸くするプロパティ

p {
    width: 200px;
    height: 80px;
    color: #fff;
    background: #999;
    border-radius: 10px;
}

2-8-6 boeder-shadow プロパティ
ボックスに影を表示させるプロパティ

#sample1 {
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
}
#sample2 {
    box-shadow: inset 5px 5px 10px rgba(0, 0, 0, 0.4);
}

2-8-7 float プロパティ
ボックスを左または右に寄せて配置し、その反対側に後続の要素が回り込むようにするプロパティ

2-8-8 clear プロパティ
floatプロパティでボックスが寄せて表示され要素が回り込んでkル状態を解除するプロパティ

2-8-9 display プロパティ
要素の表示形式を設定するプロパティ

2-8-10 visibility プロパティ
ボックスが透明になったかのように見えなくすることのできるプロパティ

2-8-11 overflow プロパティ
要素内容がボックス内に収まりきらなくなったときにどうするかを設定するプロパティ

2-8-12 clip プロパティ
ボックスをクリッピングして表示させるプロパティ
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
