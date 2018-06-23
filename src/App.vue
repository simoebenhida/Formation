<template>
  <div id="app">
    <div v-show="!join">
      <div class="bg-orange-dark min-h-sm -mt-8" style="transform: skewY(2deg)">
        <div class="min-h-sm flex justify-center items-center" style="transform: skewY(-2deg)">
          <div>
            <h1 class="text-center font-black text-5xl text-white">Laravel & Vuejs </br> Formation</h1>

            <p class="text-center font-mono font-bold text-white mt-8 py-1">
              On Friday 29 June
            </p>
            <p class="text-center font-thin text-white py-1">
              In Maison des jeunes Sidi Youssef ben Ali,Marrakech
              <a href="https://www.google.com/maps/place/%D8%AF%D8%A7%D8%B1+%D8%A7%D9%84%D8%B4%D8%A8%D8%A7%D8%A8%D8%8C+Marrakech+40000%E2%80%AD/@31.6166115,-7.9762698,17z/data=!4m5!3m4!1s0xdafee31cf0be1af:0x66f0a5f45a375c36!8m2!3d31.6154008!4d-7.9710361"
                target="__blank" class="text-sm text-white underline">(google map)</a>
            </p>
            <div class="flex flex-between justify-center items-center mt-8">
              <img class="rounded-full " src="https://pbs.twimg.com/profile_images/1009573793042501633/HCmQ27Ix_bigger.jpg" alt="">
              <p class="flex flex-col flex-start leading-normal px-2">
                <span class="font-medium text-base text-white">Mohamed Benhida</span>
                <span class="font-thin text-sm text-white">Laravel Developer</span>
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="bg-black min-h-xs -mt-8">
        <div class="min-h-xs flex justify-center items-center">
          <button @click="join = true" class="bg-orange-dark text-white py-3 px-6 text-3xl font-hairline rounded shadow hover:bg-orange-light flex items-center">
            Join Us Now
          </button>
        </div>
      </div>

      <div class="justify-center items-center flex py-4">
        <p class="text-sm text-grey-dark">Mohamed Benhida, Marrakech Formation</p>
      </div>
    </div>
    <div v-show="join" class="h-screen flex justify-center items-center">
      <div class="min-w-xs md:min-w-md rounded shadow-lg bg-white p-8">
        <!-- Begin MailChimp Signup Form -->
        <div class="font-thin text-orange-dark text-lg border-b border-orange-dark py-3">
          Join Us Now
        </div>
        <div class="flex justify-start py-8" id="mc_embed_signup">
          <form action="https://devma.us18.list-manage.com/subscribe/post?u=cfda1e0238a187ff527bdb5a5&amp;id=e718a7d58c" method="post"
            id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
            <div id="mc_embed_signup_scroll">

              <input type="email" value="" name="EMAIL" class="email" id="mce-EMAIL" placeholder="email address" required>
              <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
              <div style="position: absolute; left: -5000px;" aria-hidden="true">
                <input type="text" name="b_cfda1e0238a187ff527bdb5a5_e718a7d58c" tabindex="-1" value="" autofocus>
              </div>
              <div class="clear">
                <input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button">
              </div>
            </div>
          </form>
        </div>
        <a @click="join = false" href="#" class="text-center text-xs mt-4 underline text-orange-dark">Back To Home</a>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'app',
    data() {
      return {
        join: false
      }
    }
  }
</script>