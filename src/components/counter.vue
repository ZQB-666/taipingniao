<template>
    <div>
        <h3>{{title}}</h3>
        <button @click="sub">-</button>
        <span>{{count}}</span>
        <button @click="add">+</button>
    </div>
</template>


<script>
    export default{
        data:function(){
            return {
                count:0,
                title:"数量"
            }
        },
        methods:{
            sub:function(){
                if(this.count>0){
                this.count--;
                }
            },
            add:function(){
                this.count++;
            }
        }
    }
</script>


<style></style>