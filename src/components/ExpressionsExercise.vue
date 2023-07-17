<template>
  <div class="expression-exercises container">
    <div class="row">
      <div class="col-12">
        <h1>Exercises</h1>
        <div class="border p-1">
          <p>
            Write a math equation Vue can evaluate, inside of the curly braces
            below:
          </p>

          <p>25 x 15 = {{total}}</p>
        </div>
        <div class="border p-1">
          <p>
            Use interpolation to get the customary Hello, World! to display on
            the screen. Don't forget your quotes
          </p>
          <p>{{helloWorld()}}</p>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import { computed } from "vue";


export default{
  setup(){




    return{
      total: computed(() => {
        let total = 25 * 15
        return total
      }),

      helloWorld(){
        let quote = '"Hello World!"'
        return quote
      }


    }
  }
}


</script>

<style>


</style>