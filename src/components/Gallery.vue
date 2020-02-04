<template>
		<div class="container">
				<div class="columns is-multiline is-mobile">

								<div v-for="art in artworks" :key="art.id" class="column is-one-quarter">
										<figure class="image w-100">
												<artwork :obj="art"></artwork>
										</figure>
								</div>

				</div>
		</div>
</template>

<script>
    import Artwork from "./Artwork";
    export default {
        name: "Gallery",
        components: {Artwork},
        data() {
            return {
                artworks: [
                    {id: 1, name: 'A Modern World', image: 'A modern world.jpg', description: 'different thing'},
                    {id: 2, name: 'After Glow', image: 'Afterglow-web.jpg', description: 'something about this art peice'},
                    {id: 3, name: 'Biology', image: 'Biology 1.jpg', description: 'something about this art peice'},
                    {id: 4, name: 'Bodyclock', image: 'Bodyclock.jpg', description: 'something about this art peice'},
                    {id: 5, name: 'So this is where it went down', image: 'So this is where it went down.jpg', description: 'something about this art peice'},
                ]
            }
        },
    }
</script>

<style scoped>
.w-100{
		width: 100%;
}
</style>