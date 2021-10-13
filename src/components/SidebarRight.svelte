<script>
  import Sponsors from './Sponsors.svelte'
  import Events from './Events.svelte'
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
  </div>
</div>