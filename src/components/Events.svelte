<script>
  import Event from './Event.svelte'
</script>

<style>
  .Events h4{
    color: var(--main-color);
  }
</style>

<div class="Events Default-containers px-2">
    <div class="Events-title mb-3 text-center">
      <h4>Upcoming events</h4>
    </div>

    <div class="Events-column">
      <div class="Event">
        <Event/>
        <Event/>
        <Event/>
      </div>
    </div>
</div>