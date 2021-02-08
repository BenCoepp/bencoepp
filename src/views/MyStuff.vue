<template>
  <b-container fluid class="root">
    <b-list-group>
        <vue-scroll-snap>
        <MyStuffElement 
            class="item"
            img="@/assets/titelImage.png"
            name="Sony A6000"
            desc="My Camera now for years, basicly it is a simple mirrorless camera from sony, which allows you to make great videos and photos. I have been using it for over 1 year now, and it is still the best camera i ever had. "
            link="https://www.amazon.de/s?k=sony+alpha+6000&crid=KSY2MCLXTBTV&sprefix=sony+al%2Caps%2C175&ref=nb_sb_ss_ts-doa-p_3_7"
        />
        <MyStuffElement 
            class="item"
            img="@/assets/titelImage.png"
            name="Microsoft Sufrace Laptop 2"
            desc="This is my Laptop, I do all my writing and editing on here
            it is not the most powerfull one out there, but in my opinion still a 
            really great laptop that helped me write my first book, and hopefully
            will continue to serve me well."
            link="https://www.amazon.de/s?k=sony+alpha+6000&crid=KSY2MCLXTBTV&sprefix=sony+al%2Caps%2C175&ref=nb_sb_ss_ts-doa-p_3_7"
        />
        <MyStuffElement 
            class="item"
            img="@/assets/titelImage.png"
            name="Rode Podcast Microphone"
            desc="A few years ago I started my YouTube Channel and started
            producing videos, but i learned quickly that a bad audio quolity
            is the wearst and that I needed a better mice and this is where
            I bought this."
            link="https://www.amazon.de/s?k=sony+alpha+6000&crid=KSY2MCLXTBTV&sprefix=sony+al%2Caps%2C175&ref=nb_sb_ss_ts-doa-p_3_7"
        />
        <MyStuffElement 
            class="item"
            img="@/assets/titelImage.png"
            name="My Chair"
            desc="This is something that I bought only recently, a new chair. If you see
            it in one of my new videos, and you want to see it for yourself then check 
            it out over the link"
            link="https://www.amazon.de/s?k=sony+alpha+6000&crid=KSY2MCLXTBTV&sprefix=sony+al%2Caps%2C175&ref=nb_sb_ss_ts-doa-p_3_7"
        />
        </vue-scroll-snap>
    </b-list-group>
  </b-container>
</template>

<script>
// @ is an alias to /src
import VueScrollSnap from "vue-scroll-snap";
import MyStuffElement from '../components/MyStuffElement'
export default {
  name: "Home",
  components: {
    MyStuffElement,
    VueScrollSnap
  }
};
</script>
<style>
.root {
  height: 100vh;
  width: 100%;
  background-color: #3e5a79;
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}
.root::-webkit-scrollbar {
  display: none;
}
.scroll-snap-container {
  width: 100%;
  height: 100vh;
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}
.scroll-snap-container::-webkit-scrollbar {
  display: none;
}
.item {
  /* Set the minimum height of the items to be the same as the height of the scroll-snap-container.*/
  min-height: 400px;
  max-height: 400px;
}
</style>
