<script>
  import UserPotho from './UserPhoto.svelte'

  const userDetails =
    {
      name: 'Sam Anderson',
      Age: 26,
      profilePhoto: 'https://scontent.feoh4-3.fna.fbcdn.net/v/t1.6435-9/127117374_10225413017775737_3815254072231742375_n.jpg?_nc_cat=100&ccb=1-5&_nc_sid=09cbfe&_nc_eui2=AeE19bI-5yVUK7SutFpZunHWJ6wLAiwEawInrAsCLARrAnqS44ZXL6rQPIEhWQYj0hw&_nc_ohc=8H6N8H8UNDsAX80mduo&_nc_ht=scontent.feoh4-3.fna&oh=6aad0f7c896e1805286f20eee5274065&oe=6183BE18',
      coverPotho: 'https://arepa.s3.amazonaws.com/elmo002.jpg',
      workTitle: 'Fonder',
      description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora fugit tempore totam, voluptatem odio similique esse quibusdam nemo quod! Blanditiis.',
      email: 'samanderson@outlook.com',
      profileViews: 2.3,
      postViews: 2.3
    }
</script>

<style>
  .Profile-card{
    padding-bottom: 0;
  }
  .Profile-card-info {
    width: 100%;
  }
  .Profile-card-info span {
    font-size: 18px;
    font-weight: normal;
  }
  .Profile-card-info p{
    font-size: 14px;
  }
  .Profile-card-info p span{
    color: var(--main-color);
    font-size: inherit;
    font-weight: bold;
  }
  .Profile-card-user{
    color: var(--main-color);
  }
  .Profile-card-user h2{
    font-size: 18px;
  }
</style>
<div class="UserDetails Default-containers mt-3">
  <div class="row">
    <div class="col-6">
      <div class="Profile-card">
        <div class="Profile-card-content d-flex flex-column">
          <UserPotho/>
          <div class="Profile-card-info mt-2">
            <div class="Profile-card-user">
              <h2>SAM ANDERSON</h2>
              <span>Founder</span><br>
              <p>Colombia</p>
            </div>
            <div class="Profile-description">
              <p> <i class="fas fa-pen"></i> About me</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-6">
      <div class="Profile-card-text my-2 text-end">
        <p>Who viewed your profile-card <span>3.8K</span></p> 
        <p>Views of your post <span>3.8K</span></p> 
      </div>
    </div>
  </div>
</div>