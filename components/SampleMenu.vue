<template>
  <div>
    <h4>サンプル</h4>
    <ul>
      <li>
        <NuxtLink
          to="/sample/mustache"
        >
          マスタッシュ構文 {{}}
        </NuxtLink>
      </li>
      <li>
        <NuxtLink
          to="/sample/vif"
        >
          v-if
        </NuxtLink>
      </li>
      <li>
        <NuxtLink
          to="/sample/vfor"
        >
          v-for
        </NuxtLink>
      </li>
      <li>
        <NuxtLink
          to="/sample/vbind"
        >
          v-bind（省略形 :）
        </NuxtLink>
      </li>
      <li>
        <NuxtLink
          to="/sample/von"
        >
          v-on（省略形 @）
        </NuxtLink>
      </li>
      <li>
        <NuxtLink
          to="/sample/vmodel"
        >
          v-model
        </NuxtLink>
      </li>
      <li>
        Nested lists:
        <ul>
          <li>are unaffected by this style</li>
          <li>will still show a bullet</li>
          <li>and have appropriate left margin</li>
        </ul>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
}
</script>

<style>
</style>
