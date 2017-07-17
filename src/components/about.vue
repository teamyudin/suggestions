<template>
  <div>
    <h1>{{ msg }}</h1>
    {{ about }}
  </div>
</template>

<script>

import faker from 'faker'

export default {
  name: 'about',
  data () {
    return {
      msg: 'About Page',
      about: faker.lorem.sentences(15)
    }
  }
}
</script>

<style scoped>

</style>
