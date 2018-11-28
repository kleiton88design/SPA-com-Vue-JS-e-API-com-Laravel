<template>
	<login-template>

		<span slot="menuesquerdo">
			<img src="https://static.quizur.com/i/b/5b035c77702c13.471891555b035c775c3ff9.54480388.png" class="responsive-img">
		</span>

		<span slot="principal">
			<h2>Login</h2>
			<input type="text" placeholder="E-mail" v-model="email">
			<input type="password" placeholder="Senha" v-model="password">
			<button class="btn" v-on:click="login()">Entrar</button>	
			<router-link class="btn orange" to="/cadastro">Cadastre-se</router-link>
		</span>

	</login-template>
</template>

<script>
	import LoginTemplate from '@/templates/LoginTemplate'

	export default {
		name: 'Login',
		data () {
			return {
				email:'',
				password:''
			}
		},
		components:{
			LoginTemplate
		},
		methods:{
			login(){
				console.log("ok");
			}
		}
	}
</script>

<style scoped>

</style>
