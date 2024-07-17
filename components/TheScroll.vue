<!-- <template>
    <div class="container">
      <div ref="box" class="box">Scroll to animate me!</div>
    </div>
  </template>
  
  <script setup>
  import { onMounted, ref } from 'vue';
  const { $gsap } = useNuxtApp();
  const box = ref(null);
  
  onMounted(() => {
    $gsap.to(box.value, {
      scrollTrigger: {
        trigger: box.value,
        start: 'top center',
        end: 'bottom 100px',
        scrub: true,
        markers: true, // Remove this in production
      },
      rotation: 360,
      duration: 2,
    });
  });
  </script>
  
  <style scoped>
  .container {
    height: 200vh; /* Ensures enough scroll space */
  }
  .box {
    width: 100px;
    height: 100px;
    background-color: red;
    margin-top: 50vh; /* Center vertically in the viewport */
  }
  </style> -->

  <template>
    <div>
  
    </div>
  </template>
  
  <script setup>
  
  </script>
  
  <style lang="scss" scoped>
  
  </style>
  