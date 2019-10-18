<template>
    <div id="home">
      <vue-particles
        color="#009688"
        :particleOpacity="0.5"
        :particlesNumber="160"
        shapeType="circle"
        :particleSize="4"
        linesColor="#009688"
        :linesWidth="1"
        :lineLinked="true"
        :lineOpacity="0.4"
        :linesDistance="150"
        :moveSpeed="10"
        :hoverEffect="true"
        hoverMode="grab"
        :clickEffect="true"
        clickMode="push"
        class="landing"
      >
      </vue-particles>
    </div>
</template>

<style scoped>
  .landing {
    height: 100vh;
    background-attachment: fixed;

  }
</style>
