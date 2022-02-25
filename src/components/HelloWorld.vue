<!--
 * @Date: 2022-02-24 19:59:24
 * @LastEditors: maclerylin
 * @LastEditTime: 2022-02-24 20:03:22
-->
<template>
    <div class="vuera">
        <h1>It's a react component and it wraps a vue component, see following</h1>
        <test-react-c name="maclerylin"/>
    </div>
</template>

<script>
import Vue from 'vue'
import { VuePlugin } from 'vuera'
import TestReactC from '../react-component/TestReactC.jsx';

Vue.use(VuePlugin)


export default {
    name: 'VueRa',
    components: {
        TestReactC,
    }
}
</script>

<style scoped>
    .vuera {
        margin: 0 auto;
        text-align: left;
    }
</style>