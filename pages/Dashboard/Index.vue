<template>
    <div>
        <NavBarMenu/>
        <Dashboard/>
    </div>
</template>

<script>
import Dashboard from "~/components/Dashboard/Panel.vue";
import NavBarMenu from "~/components/Dashboard/NavBarMenu.vue";

export default {
    components: {
        Dashboard,
        NavBarMenu
    }
}
</script>