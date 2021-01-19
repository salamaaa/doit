<template>
    <div>
        <div v-for="(item,index) in items" :key="index">
            <list-item :item="item" :class="item" s/>
        </div>
    </div>
</template>

<script>
import listItem from './listItem'

export default {
    name: "listView",
    props:['items'],
    comments:{
        listItem
    }
}
</script>

<style scoped>
    .item{
        background: #e6e6e6;
        padding: 5px;
        margin-top:5px ;
    }
</style>
