<template>

	<div class="row">
		<grid-vue class="input-field" tamanho="12">
			<textarea id="conteudoID" v-model="conteudo" class="materialize-textarea"></textarea>
			<label for="conteudoID">O que esta acontencendo?</label>
		</grid-vue>
		<p>
			<grid-vue v-if="conteudo" class="btn waves-effect waves-light" tamanho="2 offset-s10">Publicar</grid-vue>
		</p>
	</div>

</template>

<script>
	import GridVue from '@/components/layouts/GridVue'
	export default {
		name: 'PublicarConteudoVue',
		props:[],
		data () {
			return {
				conteudo:''
			}
		},
		components:{
			GridVue
		}
	}
</script>

<style scoped>

</style>