<template>
	<!--{{article}}-->
			<section>
        <img src="https://images.unsplash.com/photo-1622495894321-010d1e6db2a9?ixid=MnwxMjA3fDF8MHxlZGl0b3JpYWwtZmVlZHwxfHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=700&q=60" alt="">
        <img src="https://images.unsplash.com/photo-1627340067228-14a5222671a3?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw0fHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=700&q=60" alt="">
        <img src="https://images.unsplash.com/photo-1627379429510-e32426ba200f?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwzfHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=700&q=60" alt="">
        <img src="https://images.unsplash.com/photo-1627371101470-d506fe82be62?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw1fHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=700&q=60" alt="">
        <img src="https://images.unsplash.com/photo-1593642531955-b62e17bdaa9c?ixid=MnwxMjA3fDF8MHxlZGl0b3JpYWwtZmVlZHw2fHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=700&q=60" alt="">
        <img src="https://images.unsplash.com/photo-1627000086207-76eabf23aa2e?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw3fHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=700&q=60" alt="">
        <img src="https://bad.src/not/valid" alt="">
    </section>
</template>

<script>
	const getArticle = async () => {
		await new Promise(resolve => setTimeout(resolve, 3000))
		
	// const article = {
	// 	title: 'My Vue3 Article',
	// 	author: 'Jesiel Gomes'
	// }
	
	// return article
		
	}
	
	export default{
		async setup(){
			const article = await getArticle()
			
			// return { article	}
		}
	}
</script>

<style scoped>
		section{
		max-width: 100%;
		display: flex;
		flex-wrap: wrap;
		align-items: center;
		justify-content: center ;
		background-color: #8827ba;
		margin: 0;
	}
</style>