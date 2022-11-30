<template>
    <div>
        <NavBarMenu/>
        <Dashboard/>
    </div>
</template>

<script>
import NavBarMenu from "~/components/Dashboard/NavBarMenu.vue";
import Dashboard from "~/components/Dashboard/Panel.vue";
export default {
    components: {
    Dashboard,
    NavBarMenu
}
}
</script>