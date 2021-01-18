<template>
  <div>
    <h1>Hello</h1>
    <span>{{ this.$route.params }}</span>
    <h2>{{ year }}年</h2>
    <h2>{{ month }}月</h2>
  </div>
</template>

<script>
export default {
  mounted() {
    this.$nextTick(() => {
      // const params = this.$route.params
      // console.log('Year:', params.year)
      // console.log('Month:', params.month)
      // TODO: Axios でのリクエストコードの追加
    })
  },
  // methods: {
  //   year() {
  //     return this.$route.params.year
  //   },
  // },
  computed: {
    year() {
      return this.$route.params.year
    },
    month() {
      return this.$route.params.month
    },
  },
}
</script>

<style scoped>
body {
  background: #fefefe;
}
</style>
