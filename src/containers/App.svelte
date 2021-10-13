<script>
  import Header from '../components/Header.svelte'
  import Main from '../components/Main.svelte'
  import SidebarLeft from '../components/SidebarLeft.svelte'
  import SidebarRight from '../components/SidebarRight.svelte'
  import Timeline from '../components/Timeline.svelte'

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
    border: .5px solid var(--main-color);
    border-radius: 1rem;
    padding: 1.2rem 2rem;
    margin-bottom: 1.2rem;
  }

</style>

<Header/>

<Main>
  <SidebarLeft/>
  <Timeline/>
  <SidebarRight/>
</Main>