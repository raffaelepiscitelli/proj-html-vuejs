<template>
    <li>{{ linkHeader }}</li>
</template>
<script>
export default {
    props: [
        'linkHeader'
        ]
}
</script>
<style lang="scss" scoped>
    @use '../style/general.scss' as *;
</style>