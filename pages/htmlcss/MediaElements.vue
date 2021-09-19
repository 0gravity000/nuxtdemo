<template>
  <div>
    <h3>画像・動画・音声関連の要素</h3>
<pre>
1-9-1 img要素

<img src="logo.png" alt="株式会社マイナビ" width="100" height="70">

<img src="logo.png" srcset="logo200.png 2x, logo300.png 3x" alt="株式会社マイナビ" width="100" height="70">

<img sizes="100vw" srcset="small.jpg 400w, medium.jpg 800w, large.jpg 1600w" src="small.jpg" alt="">

<img sizes="(max-width: 30em) 100vw, (max-width: 50em) 50vw, calc(33vw - 60px)" srcset="small.jpg 400w, medium.jpg 800w, large.jpg 1600w" src="small.jpg" alt="">

1-9-2 picture要素

<picture>
    <source media="(min-width: 50em)" srcset="large.jpg">
    <source media="(min-width: 30em)" srcset="medium.jpg">
    <img src="small.jpg" alt="">
</picture>

1-9-3 source要素

<picture>
    <source media="(max-width: 500px)" srcset="phone.jpg, phone-retina.jpg 2x">
    <img src="pc.jpg" srcset="pc-retina.jpg 2x" alt="">
</picture>

<picture>
    <source srcset="pic.apng" type="image/apng">
    <source srcset="pic.webp" type="image/webp">
    <img src="pic.jpg" alt="">
</picture>

<video controls>
    <source src='trip.mp4' type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'>
    <source src='trip.ogv' type='video/ogg; codecs="theora, vorbis"'>
    ・・・
</video>

1-9-4 video要素

<video src="trip.mp4" controls width="640" height="360">
    <p><a href="trip.mp4">動画ファイルをダウンロード</a></p>
</video>

1-9-5 audio要素

<audio src="song4u.mp3" controls>
    <p><a href="song4u.mp3">音声ファイルをダウンロード</a></p>
</audio>

1-9-6 track要素

<video src="trip.ogv" controls>
    <track kind="subtitles" src="trip.ja.vtt" srclang="ja" label="日本語">
    <track kind="subtitles" src="trip.en.vtt" srclang="en" label="English">
</video>

1-9-7 embed要素

<embed src="game.swf" type="application/x-shockwave-flash" width="500" height="500" quality="high">

1-9-8 map要素

<img src="map.png" usemap="#navbar" alt="ナビゲーションバー">
…
<map name="navbar">
<area href="prev.html" alt="前ページ" shape="rect" coords="100,10,170,30">
<area href="next.html" alt="次ページ" shape="rect" coords="200,10,270,30">
</map>

1-9-9 area要素

1-9-10 object要素

1-9-11 param要素

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
