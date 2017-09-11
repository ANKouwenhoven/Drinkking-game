<template>
  <div>
    <p>testing</p>
    <p>{{question}}</p>
  </div>
</template>

<script>
/* eslint-disable */
export default {
  data () {
    return {
      question: ""
    }
  },
  created: function () {
    fetch("https://opentdb.com/api.php?amount=1&type=multiple")
      .then(response => console.log(response))
  } 
  
}

</script>