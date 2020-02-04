<template>
		<img v-bind:src="'/images/' + obj.image" @click="expand">
</template>

<script>
    export default {
        name: "Artwork",
        props: {
            obj: { required: true },
        },
        data() {
            return {
            }
        },
								methods:{
            expand: function () {
												}
								}
    }
</script>

<style scoped>

</style>