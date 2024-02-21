<script>
	import Available from "./available.svelte";
	import Follow from "./follow.svelte";

</script>

<h1 class="text-7xl font-bold text-red-700">The <br> Johnny Dollar Show</h1>
<div class="hero min-h-screen ">
  <div class="hero-content flex-col lg:flex-row">
    <img src="assets/johnny-dolor.jpg" class="max-w-sm rounded-lg shadow-2xl" />
    <div class="flex-1 text-white">
          <p class="py-6"><b>The Johnny Dollar show</b> is podcast show which contains many  compilation episodes from the classic radio show Yours Truly Johnny Dollar. </p>
          <p class="py-6"><b>Get READY for your favorite heroes!</b> Here is can listen all the episodes from Yours Truly Johnny Dollar, with Bob Bailey,  
        Edmund O' Brian,  Charles Rusell , Dick Powell, John Lund, Gerald Mohr, Bob Readick, Mandel Kramer.  
      </p>
    </div>
  </div>
</div>

<Available/>

<Follow/>
