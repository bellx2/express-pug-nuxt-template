<template lang="pug">
    .container
        p TEST!
        el-radio(v-model="radio" label='A' @change="setRadio") 選択A
        el-radio(v-model="radio" label='B') 選択B
        p {{ radio }}
</template>

<script>
export default {
  data () {
    return {
      value: null,
      radio: 'A'
    }
  },
  methods: {
    setRadio () {
      console.log('radioooooooooo')
    }
  }
}
</script>

<style scoped>
.title
{
  margin: 30px 0;
}
.users
{
  list-style: none;
  margin: 0;
  padding: 0;
}
.user
{
  margin: 10px 0;
}
</style>
