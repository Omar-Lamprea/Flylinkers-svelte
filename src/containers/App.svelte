<script>
  import {onMount} from 'svelte'
  import Header from '../components/Header.svelte'
  import Main from '../components/Main.svelte'
  import SidebarLeft from '../components/SidebarLeft.svelte'
  import SidebarRight from '../components/SidebarRight.svelte'
  import Timeline from '../components/Timeline.svelte'

  //Routes
  import Profile from '../components/Profile/Profile.svelte'

  // let currentPage = [
  //   {
  //     home:[SidebarLeft, Timeline]
  //   },
  //   {
  //     profile: [Profile, SidebarRight]
  //   }
  // ]

  let currentPage = 'home'

  function changePage(newPage){
    currentPage = newPage
    // history.pushState(null, currentPage, `/${currentPage}`);
  }

  


</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300;400&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');

  :root{
    --main-color: #199AAF
  }
  :global(body){
    background-color: #fafafa;
    color: rgba(38, 38, 38, 07);
    /* font-family: 'Lato', sans-serif; */
    margin: 0;
    padding: 0;
  }
  :global(h1, h2, h3, h4, h5, h6, p){
    margin: 0;
    padding: 0;
  }

  :global(a){
    text-decoration: none;
    color: var(--main-color);
  }

  :global(.Default-containers){
    background-color: #fafafa;
    border: .5px solid var(--main-color);
    border-radius: 1rem;
    padding: 1.2rem 2rem;
    margin-bottom: 1.2rem;
  }
  :global(.Default-containers-grey){
    background-color: #EFEFEF;
    border: none;
    border-radius: 1rem;
    padding: 1.2rem 2rem;
    margin-bottom: 1.2rem;
  }
</style>

<Header />

<Main>
  <div class="nav">
    <button on:click={() =>changePage('home')}>Home</button>
    <button on:click={() =>changePage('profile')}>Profile</button>
  </div>

  <!-- <svelte:component this={currentPage.profile[0]} />
  <svelte:component this={currentPage.profile[1]} /> -->

  {#if currentPage === 'home'}
    <SidebarLeft />
    <Timeline />
    <!-- <Profile /> -->
    <SidebarRight />
  {:else if currentPage === 'profile'}
    <Profile />
    <SidebarRight />
  {/if}

</Main>