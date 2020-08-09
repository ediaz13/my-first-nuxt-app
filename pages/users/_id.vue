<template>
    <h1>A single user page, with Id : {{$route.params.id}} </h1>
</template>

<script>
export default {
    validate(data) {
        return /^\d+$/.test(data.params.id); 
    }
}
</script>