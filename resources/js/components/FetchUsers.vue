<template>
	<div>
		Obteniendo data via Api...
	</div>
</template>

<script>
import axios from 'axios'

export default {
	mounted () {
		axios.get('/api/users')
		.then(response => console.log(response.data)) 
	}
}
	
</script>