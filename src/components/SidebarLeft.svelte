<script>
  import ProfileCard from './Profile-card/ProfileCard.svelte'
  import Groups from './groups-card/Groups.svelte'
  import Hashtags from './hashtags-card/Hashtags.svelte'
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