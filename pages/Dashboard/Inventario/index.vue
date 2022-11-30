<template>
    <div>
        <NavBarMenu/>
        <Inventario/>
    </div>
</template>
<script>
import Inventario from "~/components/Dashboard/Inventario.vue";
import NavBarMenu from "~/components/Dashboard/NavBarMenu.vue";
export default {
    components: {
    NavBarMenu,
    Inventario
}
}
</script>