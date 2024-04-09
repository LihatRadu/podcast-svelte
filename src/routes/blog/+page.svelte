<script lang="ts">
  import {posts} from './posts';
</script>

<div class="text-5xl font-bold text-red-700 text-center">Blog</div>

<div class="container mx-auto px-4 py-20">
  <div class="recent-news-order grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
    {#each posts as post (post.id)}
      <div class="news-post bg-gray-700 rounded-lg shadow-md overflow-hidden">
        <div class="post p-6">
          <h2 class="post-title text-xl font-semibold mb-2">
            <a href={`/blog/${post.id}`} class="hover:text-red-700">{post.title}</a>
          </h2>
          <p class="post-meta text-gray-500 text-sm mb-4">{post.date}</p>
          <img src={post.image} alt={post.alt} class="post-image w-full h-48 object-cover mb-4" />
          <p class="post-excerpt mb-4">{post.content}</p>
          <a href={""} class="read-more text-blue-500 hover:text-blue-700">Read More</a>
        </div>
      </div>
    {/each}
  </div>
</div>
