<script>
  import ProfileCard from './ProfileCard.svelte'
  import Groups from './Groups.svelte'
  import Hashtags from './Hashtags.svelte'
</script>

<style>
  /* .Sidebar-container {
    position: fixed;
    width: 100%;
  } */
</style>

<div class="Sidebar col-3">
  <div class="Sidebar-container">
    <ProfileCard/>
    <Groups/>
    <Hashtags/>
  </div>
</div>