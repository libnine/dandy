<template>
  <div class="main">
    <h1><span id="one">dandy</span><span id="two">data</span><span id="three">dev</span></h1>
  </div>
</template>

<script>
export default {
  name: 'Headerv',
  data () {
    return {

    }
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Montserrat:100,200,300,400,500,600,700&display=swap');

.main {
  font-family: 'Montserrat', sans-serif;
}

#one {
  color:	#0C1178;
}

#two {
  color: #FA641E;
  font-weight: lighter;
}

#three {
  color: #0C1178;
  font-weight: 500;
}

h1 {
  font-size: 72px;
}

</style>