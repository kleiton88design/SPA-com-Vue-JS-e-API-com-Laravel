<template>
	<login-template>

		<span slot="menuesquerdo">
			<img src="https://static.quizur.com/i/b/5b035c77702c13.471891555b035c775c3ff9.54480388.png" class="responsive-img">	
		</span>

		<span slot="principal">
			<h2>Cadastro</h2>
			<input type="text" placeholder="Nome" value="">
			<input type="text" placeholder="E-mail" value="">
			<input type="password" placeholder="Senha" value="">
			<input type="password" placeholder="Confirme sua Senha" value="">
			<button class="btn">Enviar</button>
			<router-link class="btn orange" to="/login">Já tenho conta</router-link>
		</span>

	</login-template>
</template>

<script>
	import LoginTemplate from '@/templates/LoginTemplate'
	import CardConteudoVue from '@/components/social/CardConteudoVue'
	import CardDetalheVue from '@/components/social/CardDetalheVue'
	import PublicarConteudoVue from '@/components/social/PublicarConteudoVue'

	export default {
		name: 'Cadastro',
		data () {
			return {
				
			}
		},
		components:{
			LoginTemplate
		}
	}
</script>

<style scoped>

</style>
