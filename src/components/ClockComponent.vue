<script setup>
let t = 0;
let actualTime = 0;

function actualizar() {

 function Clock() {
    actualTime = new Date();
    t = actualTime.getHours() + ":" + actualTime.getMinutes() + ":" + actualTime.getSeconds();
    console.log(t)
     }
    setInterval(Clock, 1000);
}
actualizar();

</script>

<template>
    <p>{{t}}</p>
</template>

<style>

</style>