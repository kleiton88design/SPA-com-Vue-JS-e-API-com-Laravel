<template>
	<span>
		<div v-if="img" class="card-image">
			<img :src="img ">
			<span class="card-title">{{titulo || ''}}</span>
		</div>

		<div v-if="txt" class="card-content">
			<p>{{txt}}</p>
		</div>
	</span>
</template>

<script>
	export default {
		name: 'CardDetalheVue',
		props:['img','titulo','txt'],
		data () {
			return {

			}
		}
	}
</script>

<style scoped>

</style>
