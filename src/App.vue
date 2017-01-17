<template>
  <div id="app">
    <img src="./assets/logo.png">
    <hello></hello>

    <div class="ui icon button" data-content="Add users to your feed">
      <i class="add icon"></i>
    </div>


    <div class="ui instant move reveal">
      <div class="visible content">
        <img src="./assets/square-image.png" class="ui small image">
      </div>
      <div class="hidden content">
        <img src="./assets/chris.jpg" class="ui small image">
      </div>
    </div>



    <div class="ui basic modal">
      <div class="ui icon header">
        <i class="archive icon"></i>
        Archive Old Messages
      </div>
      <div class="content">
        <p>Your inbox is getting full, would you like us to enable automatic archiving of old messages?</p>
      </div>
      <div class="actions">
        <div class="ui red basic cancel inverted button">
          <i class="remove icon"></i>
          No
        </div>
        <div class="ui green ok inverted button">
          <i class="checkmark icon"></i>
          Yes
        </div>
      </div>
    </div>

  </div>
</template>

<script>
import Hello from './components/Hello'

export default {
  name: 'app',
  components: {
    Hello
  },
  mounted: function() {
    $('.ui.basic.modal')
      .modal('show')
    ;
  }
}


</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
