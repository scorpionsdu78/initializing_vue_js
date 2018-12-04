<<template>
  <div>  
    <h1>Clicked {{number}} tines</h1>
    <button @click="iAmClicked()">Click me!</button>
  </div>
</template>
 
<script>
    export default {

        

        data() {
            return {
              title: 'cliked 0 time',
              number: 0
              }
        },
        methods: {
            iAmClicked() {
                
                this.number = this.number + 1;
            }
        }
    };
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
