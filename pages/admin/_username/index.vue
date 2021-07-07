<template>
  <div>Username Admin : {{$route.params.username}} </div>
</template>

<script>
export default {
    validate(data) {
        return /^\d+$/.test(data.params.username);
    }
}
</script>

<style>

</style>