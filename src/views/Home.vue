<template>
  <div class="container-fluid backgroundcontent">
    <div class="row">
      <Headers />
      <Sidebar />
      <Content />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Headers from '../components/header'
import Sidebar from '../components/sidebar'
import Content from '../components/content'
export default {
  name: 'Home',
  components: {
    Headers,
    Sidebar,
    Content
  }
}
</script>

<style scoped>
.backgroundcontent {
  background: #fbfcff;
}
</style>
