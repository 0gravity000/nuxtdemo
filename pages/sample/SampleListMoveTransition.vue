<template>
  <div>
    <h3>リスト移動トランジション その1</h3>
    <button @click="shuffle">
      Shuffle
    </button>
    <transition-group name="flip-list" tag="ul">
      <li v-for="item in items" :key="item">
        {{ item }}
      </li>
    </transition-group>

    <h3>リスト移動トランジション その2</h3>
    <button @click="shuffle">
      Shuffle
    </button>
    <button @click="add">
      Add
    </button>
    <button @click="remove">
      Remove
    </button>
    <transition-group name="list-complete" tag="p">
      <span
        v-for="item in items"
        :key="item"
        class="list-complete-item"
      >
        {{ item }}
      </span>
    </transition-group>
  </div>
</template>

<script>
import _ from 'lodash'

export default {
  layout: 'LayoutSample',
  data () {
    return {
      items: [1, 2, 3, 4, 5, 6, 7, 8, 9],
      nextNum: 10
    }
  },
  methods: {
    shuffle () {
      this.items = _.shuffle(this.items)
    },
    randomIndex () {
      return Math.floor(Math.random() * this.items.length)
    },
    add () {
      this.items.splice(this.randomIndex(), 0, this.nextNum++)
    },
    remove () {
      this.items.splice(this.randomIndex(), 1)
    }
  }
}
</script>

<style scoped>
.flip-list-move {
  transition: transform 1s;
}

.list-complete-item {
  transition: all 1s;
  display: inline-block;
  margin-right: 10px;
}
.list-complete-enter, .list-complete-leave-to
/* .list-complete-leave-active for below version 2.1.8 */ {
  opacity: 0;
  transform: translateY(30px);
}
.list-complete-leave-active {
  position: absolute;
}

</style>
