<template>
    <article class="tweet border-b bborder-gray-600">
        <div class="text-white">{{ tweet.author.display_name }}</div>
    </article>
</template>

<script>
export default {
    props: ['tweet']
}
</script>