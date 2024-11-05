<template>
    <div class="sidebar" :style="{width: sidebarWidth}">
<h1>
    <span v-if="collapsed">
        <div class="logo">
            <img src="@/assets/Abdi.jpg" alt="Vue">
        </div>
    </span>
    <div class="logoFalse" v-else>
    <span><img src="@/assets/Abdi.jpg" alt="Vue"></span>
    </div>
</h1>
<span class="collapse-icon"
    :class="{ 'rotate-180': collapsed }"
    @click="toggleSidebar">
    <i class="fas fa-angle-double-left"></i>
</span>
<SidebarLink to="/" icon="fas fa-home">Home</SidebarLink>
<SidebarLink to="/about" icon="fas fa-user">About Me</SidebarLink>
<SidebarLink to="/skills" icon="fas fa-tools">Skills</SidebarLink>
<SidebarLink to="/projects" icon="fas fa-folder-open">Projects</SidebarLink>

    </div>
</template>

<script>
import SidebarLink from './SidebarLink.vue'
import {collapsed, toggleSidebar,sidebarWidth} from "./state"
export default {
props: {},
components:{SidebarLink},
setup(){
    return{collapsed, toggleSidebar, sidebarWidth}
}
}
</script>



<style>
:root{
    --sidebar-bg-color:#A0D4FF;
    --sidebar-item-hover:#4a90e2;
    --sidebar-item-active:#4a90e2;
}
</style>

<style scoped>
.sidebar{
    color:white;
    background-color: var(--sidebar-bg-color);
    float:left;
    position: fixed;
    z-index: 1;
    top: 0;
    left: 0;
    bottom:0;
    padding: 0.5em;
    transition: 0.3s ease;
    display:flex;
    flex-direction: column;
}

.collapse.icon{
    position: absolute;
    bottom: 0;
    padding: 0.75em;

    color: rgba(255,255,255,0.7);

    transition: o.2s linear;
}

.rotate-180{
    transform: rotate(180deg);
    transition: 0.2s linear;
}

.logo {
    margin-bottom: 1rem;
}
.logo img{
    width:2.4rem;
    border-radius: 20px;
}

.logoFalse{
    margin-bottom:0rem;
}

.logoFalse img{
    width:3rem;
    border-radius: 30px;
}
</style>
