<template>
	<span>
		<header>
    		<nav-bar logo="Social" url="/" cor="deep-purple darken-3">
				<li><router-link to="/">Home</router-link></li>
				<li><router-link to="/register">Registrar</router-link></li>
			</nav-bar>
    	</header>

		  <main class="deep-purple lighten-5">
			  <div class="container">
				  <div class="row">
					  <grid tamanho="8">
						  <slot name="menu"/>
					  </grid>

					  <grid tamanho="4">
						  <slot name="content"/>
					  </grid>
				  </div>
			  </div>
		  </main>

    	<Footer cor="deep-purple darken-3" logo="Social" descricao="Teste de descrição" ano="2019">
			<li><a class="grey-text text-lighten-3" href="#!">Link 1</a></li>
			<li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
			<li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
			<li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>
		</Footer>
  	</span>
</template>

<script>
import NavBar from "@/components/layouts/NavBar";
import Footer from "@/components/layouts/Footer";
import Grid from "@/components/layouts/Grid";
import CardMenu from "@/components/layouts/CardMenu";

export default {
	name: 'LoginTemplate',
	components: {CardMenu, Grid, Footer, NavBar}
}
</script>

<style>
</style>
