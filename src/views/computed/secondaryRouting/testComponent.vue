<template>
  <div class="assembly">
    <div class="ass">
        {{ comName }}
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {}
  },
  props: {
    person: {
      type: Object
    }
  },
  computed: {
    //   如果template里没用到，自然不会执行
    comName() {
        console.log('aa')
      return this.person.name
    }
  }
}
</script>
<style lang="scss" scoped>
.assembly {
    background-color: aqua;
}
</style>

