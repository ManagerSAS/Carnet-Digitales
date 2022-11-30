<template>
    <div>
        <NavBarMenu/>
        <CreateTheme/>
    </div>
</template>
<script>
import CreateTheme from "~/components/Dashboard/CreateTheme.vue";
import NavBarMenu from "~/components/Dashboard/NavBarMenu.vue";
export default {
    components: {
        NavBarMenu,
        CreateTheme
    }
}
</script>