<template>
  <div id="app">
    <div class="container">
      <div class="row mt-5">
        <div class="col-md-12">
          <button class="btn btn-outline-primary mr-1" @click="selected = 'CardComponent'">Card</button>
          <button class="btn btn-outline-danger mr-1" @click="selected = 'AboutComponent'">About</button>
          <button class="btn btn-outline-warning mr-1" @click="selected = 'ContactComponent'">Contact</button>
        </div>
      </div>
      <div class="row mt-5">
        <div class="col-md-12">
          <component :is="selected"></component>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
import CardComponent from "@/components/CardComponent";
import AboutComponent from "@/components/AboutComponent";
import ContactComponent from "@/components/ContactComponent";

export default {
  name: 'App',

  data: function () {
    return {
      title: 'Card 1',
      selected: 'CardComponent'
    }
  },
  components: {
    CardComponent,
    AboutComponent,
    ContactComponent
  }
}
</script>

<style>

</style>
