<script>
  import svelteLogo from './assets/svelte.svg'
  import Counter from './lib/Counter.svelte'
</script>

<main class="wrap mx-5">
  <h1 class="text-2xl mb-5">We help startups and enterprises design digital products that <span class="text-amber-600 font-bold">just work.</span></h1>
  <section class="grid grid-cols-1 md:grid-cols-2 gap-4">
    <!-- Article # 1 -->
    <article class="px-4 py-4 rounded-2xl card_dark transition-all hover:translate-y-2 hover:text-white card_section">
      <a class="flex text-white" href="www.google.com">
        <div class="flex flex-col justify-between w-1/2">
          <div class="flex">
            <span class="cases-card__tag-icon">
              <svg class="svg-icon" viewBox="0 0 30 30"><use xlink:href="#svg-icon-travel"></use></svg>
            </span>
            <h4>Travel</h4>
          </div>
          <div>
            <h4 class="text-xl font-bold mb-2">Finding space <br> with NASA</h4>
            <p class="text-xs">We helped the original moonshot organization create a new storage optimization system for the International Space Station.</p>
          </div>
        </div>
        <div class="card_toggle w-7/12 card_img ">
          <img class="card_item static_img" src="./images/static_nasa2.png" alt="">
          <img class="card_item animated_img" src="./images/animated_nasa.gif" alt="">
        </div>
      </a>
    </article>
    <!-- Article #2 -->
    <article class="px-4 py-4 rounded-2xl card_light transition-all hover:translate-y-2 card_section">
      <a class="flex" href="www.google.com">
        <div class="flex flex-col justify-between w-1/2">
          <div class="flex">
            <span class="cases-card__tag-icon">
              <svg class="svg-icon" viewBox="0 0 30 30"><use xlink:href="#svg-icon-travel"></use></svg>
            </span>
            <h4>Fintech</h4>
          </div>
          <div>
            <h4 class="text-xl font-bold mb-2">From zero to MVP<br> with Strovoo</h4>
            <p class="text-xs">The founders of this fine Silicon Valley gig economy startup came to Humbleteam with an insight and an idea. Two months later they had a working MVP and a marketing site, ready to go.</p>
          </div>
        </div>
        <div class="card_toggle card_img w-10/12 transition-all">
          <img class="card_item static_img" src="./images/static_pig.png" alt="">
          <img class="card_item animated_img" src="./images/animated_pig.gif" alt="">
        </div>
      </a>
    </article>
    <!-- Article #3 -->
    <article class="px-4 py-4 rounded-2xl card_light transition-all hover:translate-y-2 card_section">
      <a class="flex" href="www.google.com">
        <div class="flex flex-col justify-between w-1/2">
          <div class="flex">
            <span class="cases-card__tag-icon">
              <svg class="svg-icon" viewBox="0 0 30 30"><use xlink:href="#svg-icon-travel"></use></svg>
            </span>
            <h4>Travel</h4>
          </div>
          <div>
            <h4 class="text-xl font-bold mb-2">Welcome aboard <br> Royal Caribbean</h4>
            <p class="text-xs">When the world’s biggest cruise company asked us to redesign their app we saw it as an opportunity to make millions of passengers a little bit happier.</p>
          </div>
        </div>
        <div class="card_toggle card_img w-10/12 transition-all -rotate-12">
          <img class="card_item static_img" src="./images/static_drink.png" alt="">
          <img class="card_item animated_img" src="./images/animated_drink.gif" alt="">
        </div>
      </a>
    </article>
    <!-- Article #4 -->
    <article class="px-4 py-4 rounded-2xl card_dark transition-all hover:translate-y-2 hover:text-white card_section">
      <a class="flex text-white" href="www.google.com">
        <div class="flex flex-col justify-between w-1/2">
          <div class="flex">
            <span class="cases-card__tag-icon">
              <svg class="svg-icon" viewBox="0 0 30 30"><use xlink:href="#svg-icon-travel"></use></svg>
            </span>
            <h4>Automotive</h4>
          </div>
          <div>
            <h4 class="text-xl font-bold mb-2">Always alert<br> with Nexar</h4>
            <p class="text-xs">Funded by Samsung and Alibaba, Nexar makes the world’s smartest dashcams. We helped design their web and mobile apps.</p>
          </div>
        </div>
        <div class="card_toggle card_img -rotate-12">
          <img class="card_item static_img" src="./images/static_hand.png" alt="">
          <img class="card_item animated_img" src="./images/animated_hand.gif" alt="">
        </div>
      </a>
    </article>
    
  </section>
</main>

<style>
  .card_dark { background-color: #1d1d1b; }
  .card_light { 
    background-color: white;
    color: #1d1d1b !important;
    border: #1d1d1b 3px solid;
   }
  .card_toggle { 
    align-self: flex-start;
    position: relative;
    pointer-events: none;
  }
  .card_img {
    width: 65%;
    margin: -12% -19% 0 -7%;
  }

  .card_section:hover .card_img .card_item.animated_img  { opacity: 1; }
  .card_section:hover .card_img .card_item.static_img  { opacity: 0; }
  .card_section .card_img .card_item.animated_img { opacity: 0; }

  .card_toggle::after {
    content: '';
    display: block;
    position: relative;
    width: 100%;
    padding-bottom: 100%;
    height: 0;
  }
  .card_item {
    position: absolute;
    width: 100%;
    height: 100%;
    opacity: 1;
    object-fit: contain;
  }
</style>
