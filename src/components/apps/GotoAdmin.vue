<!--
 * @Author: Royal
 * @LastEditTime: 2021-09-18 18:48:54
 * @Description: 
 * @FilePath: /publishTest/src/components/apps/GotoAdmin.vue
-->
<template>
    <div>Loading</div>
</template>
<script lang="ts" setup>

import { DWM } from 'vue3-win10'
import { inject } from "vue"

let winId = <string>inject('windowId')
setTimeout(() => {
    window.open('https://github.com/royalknight56/vue-windows10')
})
setTimeout(() => {
    if (winId) {
        DWM.getInstance().destoryWindow(winId)
    }
},1000)


</script>

<style scoped>
.t2 {
    z-index: 99;
    background-color: blanchedalmond;
}
.t2:hover {
    background-color: rgba(255, 235, 205, 0.747);
}
</style>