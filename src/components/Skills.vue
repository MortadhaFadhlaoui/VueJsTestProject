<template>
  <div class="hello">
    <div class="holder">
      <ul>
        <li v-for="(data, index) in skills" :key="index">
          {{index}}. {{data.skill}}
        </li>
        <div v-bind:class="{ alert : showAlert }"></div>
        <!--<p v-if="skills.length > 1"> You have more then one skills</p>
        <p v-else> You have less than or equal to 1 skill</p>-->
      </ul>
    </div>
    <!--{{ name }}
    <br/>
    {{btnState ? 'Disabled' : 'Enabled'}}
    <button v-on:click="changeName" v-bind:disabled="btnState">Change Name</button>-->
  </div>
</template>

<script>
export default {
  name: 'Skills',
    data(){
      return{
         // name: 'Mortadha',
         // btnState: true,
          skills:[
              {
                  "skill": "Android"
              },
              {
                  "skill": "IOS"
              }
          ],
          showAlert: true
      }
    },
    methods: {
      /*changeName: function () {
          console.log("Changed");
      }*/
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
