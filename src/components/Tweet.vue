<template>
    <article class="tweet border-b bborder-gray-600">
        <router-link to="#" class="flex p-4">
            <figure class="w-16 mr-3">
                <img :src="tweet.author.profile_img_url" alt="image" class="rounded-full w-full" />
            </figure>

            <section class="flex-1">
                <div>
                    <span class="text-white font-bold">{{ tweet.author.display_name }}</span>
                    <span class="text-gray-500 ml-2 font-normal">{{ tweet.author.username }}</span>
                </div>

                <div :class="(tweet.image ? 'mb-3' : '')">
                    <p class="text-white">{{ tweet.body }}</p>
                </div>
            </section>
        </router-link>
    </article>
</template>

<script>
export default {
    props: ['tweet']
}
</script>