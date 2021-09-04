<template>
  <div>
    <h3>v-for</h3>
    <h4>配列のv-for その1</h4>
    <ul>
      <li v-for="todo in todos" :key="todo.text">
        {{ todo.text }}
      </li>
    </ul>
    <h4>配列のv-for その2</h4>
    <p>2番目の引数としてindexを提供できます</p>
    <ul>
      <li v-for="(todo, index) in todos" :key="todo.text">
        {{ index }}：{{ todo.text }}
      </li>
    </ul>

    <h4>オブジェクトのv-for その1</h4>
    <ul>
      <li v-for="value in object" :key="value">
        {{ value }}
      </li>
    </ul>

    <h4>オブジェクトのv-for その2</h4>
    <p>2番目の引数としてプロパティ名（すなわちキー）を提供できます</p>
    <ul>
      <li v-for="(value, name) in object" :key="value">
        {{ name }}：{{ value }}
      </li>
    </ul>

    <h4>オブジェクトのv-for その3</h4>
    <p>3番目の引数としてindexを提供できます</p>
    <ul>
      <li v-for="(value, name, index) in object" :key="value">
        {{ index }}. {{ name }}：{{ value }}
      </li>
    </ul>
    <p>オブジェクトを反復処理するとき、順序は Object.keys() の列挙順のキーに基づいており、全ての JavaScript エンジンの実装で一貫性が保証されていません。</p>
    <a :href="keyattrlink">key属性の詳細な使い方 key API ドキュメント </a>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      todos: [
        { text: 'Learn JavaScript' },
        { text: 'Learn Vue' },
        { text: 'Build something awesome' }
      ],
      object: {
        title: 'How to do lists in Vue',
        author: 'Jane Doe',
        publishedAt: '2016-04-10'
      },
      keyattrlink: 'https://jp.vuejs.org/v2/api/#key'
    }
  }
}
</script>
