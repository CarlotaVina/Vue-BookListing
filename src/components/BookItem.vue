<template>
<ul>
 <li v-for="book in books" :key="book.title">
    {{book.title}}:{{book.author}}
</li>
</ul>
    
</template>
<script>
export default {
    name: "BookItem",
    props: ["book"]    
}
</script>
   

<style>
 ul {
        list-style-type: none;
        padding: 0;
    }
    li {
        display: block;
        margin: 0 10px;
    }
    
</style>