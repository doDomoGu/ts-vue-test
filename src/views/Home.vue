<template>
  <div class="home">
    <HelloWorld msg="Well" />
    <Name />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Name from '@/components/Name.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Name
  }
}
</script>
