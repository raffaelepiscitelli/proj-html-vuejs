<template>
    <li>{{ linkFooter }}</li>
</template>
<script>
export default {
    props: [
        'linkFooter'
        ]
}
</script>
<style lang="scss" scoped>
    @use '../style/general.scss' as *;
</style>