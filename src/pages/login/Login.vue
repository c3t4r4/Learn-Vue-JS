<template>
	<login-template>
		<span slot="menu">
			<div class="card card-content">
			<grid tamanho="4">
				<img
					src="https://www.carbon-pixel.com/media/1317/article-networking.jpg?anchor=center&mode=crop&width=750&height=486&rnd=131824282130000000"
					alt=""
					class="circle responsive-img">
			</grid>
			</div>
		</span>

		<span slot="content">
			<div class="row card">
				<div class="card-content">
					<div class="row">
						<input type="email" placeholder="E-mail" value="">
						<input type="password" placeholder="Senha" value="">
						<button class="btn">Entrar</button>
						<router-link class="btn orange" to="/register">Cadastrar</router-link>
					</div>
				</div>
			</div>
		</span>
	</login-template>
</template>

<script>
import LoginTemplate from "@/templates/LoginTemplate";

export default {
	name: 'Login',
	data() {
		return {
		}
	},
	components: {
		LoginTemplate
	}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
