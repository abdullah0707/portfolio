<template>
  <div
    class="custom-section h-screen uppercase lg:text-4xl md:text3xl sm:text2xl text-white flex justify-center items-center flex-col">
    <div class="w-fit">
      <div class="showup text-center">CREATIVE</div>
      <div class="slidein text-center">
        <h6 style="letter-spacing: .6em;">developer</h6>
      </div>
      <p class="slogan mx-auto w-fit">
        sensible to front-end
        <span>
        </span>
      </p>
    </div>
  </div>
  <div class="shadow-title">Welcome to Portfolio</div>
</template>

<script setup>
  useHead({
    titleTemplate: "%s Home",
  })
  definePageMeta({
    layout: 'app'
  })
</script>
<style scoped>
  .showup {
    animation: showup 7s ;
  }

  .slidein {
    animation: slidein 7s;
  }

  @keyframes showup {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }

  @keyframes slidein {
    0% {
      margin-left: -300%;
      opacity: 0;
    }
    100% {
      margin-left: 0%;
      opacity: 1;
    }
  }

  .slogan {
  position: relative;
  overflow: hidden;
  height: 1.25em;
  width: 0em;
  border-right: .125em solid #39F;
  box-sizing: content-box;
  letter-spacing: .15em;
  white-space: nowrap;
  animation-name: blink-start,typing, blink-end;
  animation-duration: 1s, 3.5s, 1s;
  animation-timing-function: linear, steps(40, end), linear;
  animation-delay: 1s,1s, 2s;
  animation-iteration-count: 1, 1, infinite;
  animation-direction: normal;
  animation-fill-mode: forwards;

}

.slogan span {
  overflow: hidden;
}

@keyframes typing {
  from { width: 0; }
  to   { width: 100%; }
}

@keyframes blink-start {
  from, to { border-color: #39F; }
  50% { border-color: transparent; }
}

@keyframes blink-end {
  from, to { border-color: #39F; }
  100% { border-color: transparent; }
}
</style>