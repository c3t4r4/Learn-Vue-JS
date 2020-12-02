<template>
	<div class="row">
		<div class="card">
			<div class="card-content">
				<div class="row valign-wrapper">
					<grid tamanho="1">
						<img :src="perfil" :alt="nome" class="circle responsive-img">
					</grid>
					<grid tamanho="11">
						<span class="black-text">
							<strong>{{ nome }}</strong> - <small>{{ data }}</small>
						</span>
					</grid>
				</div>
				<slot />

			</div>
			<div class="card-action">
				<p>
					<a href="javascript:void(0);"><i class="material-icons">favorite_border</i></a>
					<a href="javascript:void(0);"><i class="material-icons">insert_comment</i></a>
				</p>
			</div>
		</div>
	</div>

</template>

<script>
import Grid from "@/components/layouts/Grid";
export default {
	name: 'CardBox',
	props: [
		'perfil',
		'nome',
		'data'
	],
	data() {
		return {

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
