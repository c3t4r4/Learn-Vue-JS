<template>
	<social-template>
		<span slot="menu">
			<card-menu>
				<div class="row valign-wrapper">
					<grid tamanho="4">
						<img src="http://archives.materializecss.com/0.100.2/images/yuna.jpg" alt="" class="circle responsive-img">
					</grid>
					<grid tamanho="8">
						<span class="black-text">
							<h5>Maria Silva</h5>
							Add the "circle" class to it to make it appear circular.
						</span>
					</grid>
				</div>
			</card-menu>
			<card-menu>
				<h4>Teste</h4>
			</card-menu>
		</span>

		<span slot="content">
			<publish-content />

			<card-box
				perfil="http://archives.materializecss.com/0.100.2/images/yuna.jpg"
				nome="Maria Silva"
				data="30/11/2020 18:11h">
				<card-content
					image="http://archives.materializecss.com/0.100.2/images/sample-1.jpg"
					title="Quintal">
						<p>I am a very simple card. I am good at containing small bits of information.
						I am convenient because I require little markup to use effectively.</p>
				</card-content>
			</card-box>
		</span>
	</social-template>
</template>

<script>
import SocialTemplate from "@/templates/SocialTemplate";
import CardBox from "@/components/social/CardBox";
import CardContent from "@/components/social/CardContent";
import PublishContent from "@/components/social/PublishContent";
import CardMenu from "../../components/layouts/CardMenu";
import Grid from "../../components/layouts/Grid";

export default {
	name: 'Home',
	data() {
		return {}
	},
	components: {
		Grid,
		CardMenu,
		SocialTemplate,
		PublishContent,
		CardContent,
		CardBox
	}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
