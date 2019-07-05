<template>
    <div v-bind:class="defineClasse">
        <label for=""> {{label}} </label>
        <input class="form-control" type="text" v-on:input="$emit('input', $event.target.value)">
    </div>

</template>

<script>
  export default {
    props: ['label','tamanho'],
    data() { teste
        return {
            
        }
    },
     mounted() {
            console.log('Component mounted.')
        },
    computed: {
        defineClasse: function(){
            return "form-group "+ (this.tamanho || "form-group col-md-6 col-lg-6");
          },
    },
    methods: {
        
    }
    }
</script>
