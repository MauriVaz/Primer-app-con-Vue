<template>
    <div id="add-container" >
        <form>
            <input type="text" />
        </form>
    </div>
</template>

<script>

export default {
    name:'TodoAdd'
}
</script>

<style scoped>
#add-container{
    padding: 10px;
}
input{
    padding:10px;
    outline:none;
    border:solid 1px #ccc;
    width:100%;
}
</style>
