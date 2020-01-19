<template>
  <div class="home">
    <p class="models">
        <b-dropdown variant="light" split :text="selectedSymptom" v-model="selectedSymptom">
          <b-dropdown-item v-for="(s, index) in symptoms" :key="index" @click="selectedSymptom=s">{{ s }}</b-dropdown-item>
        </b-dropdown>
    </p>
  </div>
</template>

<script>
export default {
  name: 'Linear',
  data () {
    return {
      selectedSymptom: "Symptoms",
      symptoms: [
        "Anxiety",
        "Nausea"
      ]
    }
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Montserrat:100,200,300,400,500,600,700&display=swap');

a, a:visited {
  color: rgb(20, 119, 81);
  font-size: 20px;
  padding: 1%;
  position: relative;
  text-decoration: none;
}

a:after, a:visited:after {
  content: '';
  height: 2px;
  position: absolute;
  bottom: 0;
  left: 0;
  width: 0%;
  background: #0C1178;
  transition: 0.2s;
}

a:hover {
  color: #FA641E;
  text-decoration: none;
}

a:hover:after, a:visited:hover:after {
  text-decoration: none;
  width: 100%;
}

a.block, a:visited.block {
  display: block;
  padding: 0.5em;
}

a.block:hover, a:visited.block:hover {
  background: #eee;
}

#blocks {
  font-size: 24px;
}

::v-deep b-dropdown {
  background-color: #0C1178;
  color:orange;
  width: 200px;
}

.home {
  color: #0C1178;
  font-family: 'Montserrat', sans-serif;
  margin-top: 5%;
}

.models {
  padding: 2%;
  margin: 2%;
}

#view {
  font-weight: 300;
}

</style>
