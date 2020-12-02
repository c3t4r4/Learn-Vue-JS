<template>
	<register-template>
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
						<input type="text" placeholder="Nome" value="">
						<input type="email" placeholder="E-mail" value="">
						<input type="password" placeholder="Senha" value="">
						<input type="password" placeholder="Confirme sua Senha" value="">
						<button type="button" class="btn">Enviar</button>
						<router-link class="btn orange" to="/login">Logar</router-link>
					</div>
				</div>
			</div>
		</span>
	</register-template>
</template>

<script>
import RegisterTemplate from "@/templates/RegisterTemplate";

export default {
	name: 'Register',
	data() {
		return {
			register: false
		}
	},
	components: {
		RegisterTemplate
	}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
