<template>
    
        <Navbar></Navbar>
        <div class="d-flex">
            <div class="col-4">
                <EntryList></EntryList>
            </div>
            <div class="col">
                <router-view></router-view>
            </div>
        </div>
    
</template>
<script lang="js">

import {defineAsyncComponent} from 'vue'

export default {
    components:{
        Navbar: defineAsyncComponent (() => import('../components/Navbar.vue')),
        EntryList: defineAsyncComponent (() => import('../components/EntryList.vue')),
    }
}
</script>