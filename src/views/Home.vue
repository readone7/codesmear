<template>
  <div class="container flexContainer flexColumn fullHeight blueBackground">
    <div class="flexContainer greetings flexItem">
      <p>Hello, I'm Otun Ridwan. I'm a Fullstack Software developer based in Lagos; I speak with computers using web technologies majorly. </p> 
    </div>
    <div class="flexItem main ">
      <vue-typer 
        :text= "['I love Ruby & Ruby on Rails', 'I cant do without Javascript', 'Elixir is a really cool functional language, and i love every bit of it', 'I build blazing fast API with Phoenix', 'I love Vue JS', 'Embedded systems? Yes with Nerves and Raspberry pi' ]"
        :repeat= "Infinity"
        :shuffle= "true"
        :initial-action= "typing"
        :pre-type-delay= '70'
        :type-delay= '100'
        :pre-erase-delay= '2000'
        :erase-delay= '200'
        :erase-style= 'backspace'
        caret-animation= 'blink' >
      </vue-typer>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "home",
  
};
</script>

<style lang="scss" scoped>
.flexContainer {
  display: flex;
  margin: 4em;
}
.flexItem {
  flex: 1
}
.flexColumn {
  flex-direction: column;
}
.fullHeight {
  height: 100vh;
}
.main {
  align-self: center;
  font-size: 1.5em;
  font-weight: 600;
}

.greetings {
  align-self: center;
  font-size: 2em;
}
</style>

