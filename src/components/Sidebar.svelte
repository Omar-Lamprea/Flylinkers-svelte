<script>
  import Profile from './ProfileCard.svelte'
  import Stories from './Stories.svelte'
  import Footer from './Footer.svelte'
</script>

<style>
  .Sidebar {
    position: relative;
    /* padding: 4.5em 0 0 0; */
  }
  .Sidebar-container {
    position: fixed;
  }
</style>

<div class="Sidebar col-2">
  <div class="Sidebar-container">
    <Profile/>
    <Stories/>
    <Footer/>
  </div>
</div>