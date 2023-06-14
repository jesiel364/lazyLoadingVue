<script>
import Comp from "@/components/Comp.vue"

export default{
	
components: {
	Comp
},
	
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
		<div class="efeito-carregamento">
		</div>
	</div>
	</template>
</Suspense>





 </div>
</template>

<style>
	section{
		width: 100%;
		display: flex;
		flex-wrap: wrap;
		align-items: center;
		justify-content: center ;
		background-color: #8827ba;
		margin: 0;
	}
	
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
	
	div.efeito-carregamento{
		width: 35px;
		height: 35px;
		border-radius: 100%;
		background-color : white;
		
		animation: efeito 0.5s infinite;
	}
	
	@keyframes efeito {
		0%{
			box-shadow: 0 0 0 0 white;
		}
		100%{
			box-shadow: 0 0 0 15px rgba(255, 255, 255, 0.1);
		}
	}
</style>
