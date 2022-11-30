<template>
    <div>
        <NavBarMenu/>
        <CreateCard/>
    </div>
</template>
<script>
import CreateCard from "~/components/Dashboard/CreateCard.vue";
import NavBarMenu from "~/components/Dashboard/NavBarMenu.vue";
export default {
    components: {
        NavBarMenu,
        CreateCard
    }
}
</script>