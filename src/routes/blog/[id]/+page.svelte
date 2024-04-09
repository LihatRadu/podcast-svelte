<script context="module">
  import {posts} from '../posts';

  export async function load({ params }) {
    // Fetch the post data based on the id
    const post = posts.find((post) => post.id === params.id);
    return { post };
  }
</script>

<script lang="ts">
  export let data;
  const { post } = data;
</script>

{#if post}
  <h1 class="text-3xl font-bold mb-4">{post.title}</h1>
  <p class="text-gray-500 mb-4">{post.meta}</p>
  <img src={post.image} alt={post.alt} class="w-full h-48 object-cover mb-4" />
  <div class="post-content mb-4">
    {@html post.content}
  </div>
  <a href="/" class="text-blue-500 hover:text-blue-700">Back to Home</a>
{/if}
