<template>
    <div>
        <NavBarMenu/>
        <GenerateReport/>
    </div>
</template>
<script>
import GenerateReport from "~/components/Dashboard/GenerateReport.vue";
import NavBarMenu from "~/components/Dashboard/NavBarMenu.vue";
export default {
    components: {
        NavBarMenu,
        GenerateReport
    }
}
</script>