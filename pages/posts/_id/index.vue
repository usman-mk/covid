<template>
	<div class="container">
		<div>
			<h1 class="title">Posts page : {{ $route.params.id }}</h1>
		</div>
	</div>
</template>

<script>
export default {
    validate(context) {
        return /^\d+$/.test(context.params.id)
    }
}
</script>
