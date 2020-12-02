<template>

	<div class="row card">
		<div class="card-content">
			<div class="row">
				<grid class="input-field" tamanho="12">
					<textarea v-model="content" id="ConteudoID" class="materialize-textarea"></textarea>
					<label for="ConteudoID">O que está acontecendo ?</label>
				</grid>

				<grid v-if="content" class="btn waves-effect waves-light" tamanho="3 offset-l9">Publicar
					<i class="material-icons right">send</i>
				</grid>
			</div>
		</div>
	</div>

</template>

<script>
import Grid from "@/components/layouts/Grid";
export default {
	name: 'PublishContent',
	props: [
		'perfil',
		'nome',
		'data'
	],
	data() {
		return {
			content: ''
		}
	},
	components: {
		Grid
	}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
