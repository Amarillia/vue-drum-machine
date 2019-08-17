<template>
  <div id="app">
    <h1>Drum Machine</h1>
    <div id="drum-machine">
      <div id="display">
        <AppDrumPad msg="Q"></AppDrumPad>
        <AppDrumPad msg="W"></AppDrumPad>
        <AppDrumPad msg="E"></AppDrumPad>
        <AppDrumPad msg="A"></AppDrumPad>
        <AppDrumPad msg="S"></AppDrumPad>
        <AppDrumPad msg="D"></AppDrumPad>
        <AppDrumPad msg="Z"></AppDrumPad>
        <AppDrumPad msg="X"></AppDrumPad>
        <AppDrumPad msg="C"></AppDrumPad>
      </div>
    </div>
  </div>
</template>

<script>
import AppDrumPad from "./components/AppDrumPad.vue";

export default {
  name: "app",
  components: {
    AppDrumPad
  },

};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Bubbler+One&display=swap");

* {
  margin: 0;
  padding: 0;
  background-color: #a6592d;
}

#app {
  font-family: "Bubbler One", sans-serif;
  font-weight: 100;
  text-align: center;
}
#drum-machine {
  width: 80%;
  margin: 0 auto;
}

#display {
  display: grid;
  grid-template-columns: 125px 125px 125px;
  grid-template-rows: 125px 125px 125px;
  grid-column-gap: 15px;
  grid-row-gap: 15px;
  justify-content: center;
  background-color: #f2913d;
  border-radius: 25px;
  padding: 15px;
}

h1 {
  font-size: 50px;
  margin: 25px;
  color: #fff;
}
</style>
