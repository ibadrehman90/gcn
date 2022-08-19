<template>
  <Header />
  <Topbar />
  <Videos />
  <BottomNav />
</template>

<script>
import Header from './components/Header.vue'
import Topbar from './components/Topbar.vue'
import Videos from './components/Videos.vue'
import BottomNav from './components/BottomNav.vue'
import SearchModal from './components/SearchModal.vue'


export default {
  name: 'App',
  components: {
    Header,
    Topbar,
    Videos,
    BottomNav,
    SearchModal
  }, data() {
    return {
      modalOpen: false
    }
  },
  methods: {
    openModal() {
      console.log("works")
      this.modalOpen = !this.modalOpen;
    }
  }
}
</script>

<style scoped>


.fot{
  position: fixed;
  bottom: 0;
}

</style>
