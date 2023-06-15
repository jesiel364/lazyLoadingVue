<script>
import Comp from "@/components/Comp.vue"
import Logo from "@/assets/logo.svg"

export default{
	
components: {
	Comp
},

data(){
	return {
		Logo: Logo
	}
}
	
}

</script>

<template >
	<div id="container">
<Suspense>
	<template #default>
		<Comp />
	
	</template>
	<template #fallback>
		<div  class="pre-carregamento">
		<!-- <div class="efeito-carregamento"> -->
			<img class="svg"  :src="Logo" />
		<!-- </div> -->
	</div>
	</template>
</Suspense>





 </div>
</template>

<style>

	
	img{
		width: 55%;
		object-fit: contain ;
		border-radius : 5px;
		margin: 2% 0;
		
	}
	
	div.pre-carregamento{
		width: 100%;
		min-height: 100vh;
		position: fixed;
		top: 0;
		left: 0;
		background-color: #8827ba;
		
		transition: 0.5s;
		display: flex;
		align-items: center;
		justify-content: center;
		
		/*display: none;*/
	}

	.svg{
		width: 50px;
		margin: auto;
		display: flex;
		animation: efeito 0.5s infinite;
	}
	
	div.efeito-carregamento{
		width: 35px;
		height: 35px;
		border-radius: 100%;
		background-color : white;
		
/*		animation: efeito 0.5s infinite;*/
	}
	
	@keyframes efeito {
		0%{
			box-shadow: 0 0 0 0 white;
		}
		100%{
			width: 35px;
			box-shadow: 0 0 0 15px rgba(255, 255, 255, 0.1);
		}
	}
</style>
