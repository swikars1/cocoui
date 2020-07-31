<template>
    <div class="card">
        <div class="card-header">
            <img  :src="imageUrl" />
            <a href="#">{{ label }}</a>
        </div>
        <div v-html="desc" />
    </div>
</template>
<script>

export default {
    props: {
        imageUrl: {
            type: String,
            requird: true,
        },
        label: {
            type: String,
            required: true,
        },
        desc: {
            type: String,
            default: "",
        }
    }
};
</script>
