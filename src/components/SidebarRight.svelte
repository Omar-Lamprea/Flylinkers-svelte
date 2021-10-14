<script>
  import Sponsors from './sponsors-card/Sponsors.svelte'
  import Events from './events-card/Events.svelte'
  import People from './People/People.svelte'
</script>

<style>
  /* .Sidebar-container {
    position: fixed;
    width: 100%;
  } */
</style>

<div class="Sidebar col-3">
  <div class="Sidebar-container">
    <Events/>
    <Sponsors/>
    <People/>
  </div>
</div>