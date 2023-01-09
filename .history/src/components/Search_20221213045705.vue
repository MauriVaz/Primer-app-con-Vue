<template>
    <div id="search-container">
        <input type="text" />
    </div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name:'Search',
    data(){
        return{
            query:""
        }
    }
}
</script>

<style scoped>
    #search-container{
        width: 600px;
        margin: 0 auto;
    }

    input{
        padding: 10px;
        width:100%;
        outline: none;
    }
</style>