<template>
    <h3>Login</h3>
</template>

<script setup>
import { useUserStore } from '../stores/user-store'

const { token } = useUserStore()
</script>