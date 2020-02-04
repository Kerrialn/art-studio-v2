<template>
		<div id="app">
				<tabs>
						<tab name="Gallery" :selected="true">
        <gallery></gallery>
						</tab>
						<tab name="Exhibitions">
								<exhibitions></exhibitions>
						</tab>
						<tab name="About">
								<about></about>
						</tab>
						<tab name="Contact">
								<contact></contact>
						</tab>
				</tabs>
		</div>
</template>

<script>

    import Tabs from "./components/Tabs";
    import Tab from "./components/Tab";
    import Gallery from "./components/Gallery";
    import About from "./components/About";
    import Contact from "./components/Contact";
    import Exhibitions from "./components/Exhibitions";

    export default {
        name: 'app',
        components: {Exhibitions, Contact, About, Gallery, Tab, Tabs},
    }
</script>

<style>

		.tabs ul {
				justify-content: center;
		}

		.tabs li a {
				font-size: 18px;
		}

		.tabs li.is-active a {
				border-bottom-color: #333;
				color: #000;

		}

		#app {
				font-family: 'Avenir', Helvetica, Arial, sans-serif;
				-webkit-font-smoothing: antialiased;
				-moz-osx-font-smoothing: grayscale;
				text-align: center;
				color: #2c3e50;
		}

		.side-bar {
				top: 0;
				position: -webkit-sticky;
				position: sticky;
				z-index: 1000;
				height: calc(100vh);
				background-color: #2c3e50;
		}


		.main {
				height: 100vh;
		}
</style>
