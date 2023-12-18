<template>
    <div>
        <p>This is index page</p>
    </div>
</template>

<script setup>
const content = await queryContent('/').findOne();
useHead({ title: content.title });

</script>