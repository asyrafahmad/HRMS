<template>
    <div>
        <h1 ref="myref">Hook tutorial</h1>
        <h2>My name is: {{name}}</h2>
    </div>
</template>


<script>

export default{
    data(){
        return {
            name: 'asyraf'
        }
    },

    beforeCreate(){
        console.log(this.name)
    },

    created(){  //call mostly initial data ,from it
    console.log('created named', this.name)
    },

    mounted(){
        console.log(this.$refs.myref);
    }
}

</script>
