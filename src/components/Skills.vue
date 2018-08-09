<template>
  <div class="hello">
    <div class="holder">
      <ul>
        <li v-for="(data, index) in skills" :key="index">
          {{index}}. {{data.skill}}
        </li>
        <p v-if="skills.length > 1"> You have more then one skills</p>
        <p v-else> You have less than or equal to 1 skill</p>
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
          ]
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
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
