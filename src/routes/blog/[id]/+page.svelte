<script context="module" lang="ts">
  import { posts } from '../posts';

  export async function load({ params }: {params: {id: string}}) {
    // Ensure params.id is a string and that it exists in the posts array
    const post = posts.find((post) => post.id === params.id);
    if (!post) {
      return { status: 404 }; // Return a 404 status if the post is not found
    }
    return { post };
  }
</script>

<script lang="ts">
  export let data : { post: { title: string; date: string; image: string; alt: string; content: string } };
  
</script>

{#if data.post}
  <h1 class="text-3xl font-bold mb-4">{data.post.title}</h1>
  <p class="text-gray-500 mb-4">{data.post.date}</p>
  <img src={data.post.image} alt={data.post.alt} class="w-full h-48 object-cover mb-4" />
  <div class="post-content mb-4">
    {@html data.post.content}
  </div>
  <a href="/" class="text-blue-500 hover:text-blue-700">Back to Home</a>
{:else}
  <p>Post not found</p>
{/if}
