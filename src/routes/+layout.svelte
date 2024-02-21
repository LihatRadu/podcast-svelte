<script>
  import '../app.css';
</script>

<html data-theme="dim"></html>
 <header>
    <div>
      <img src="../../assets/The Johnny Dollar Show.png" alt="Johnny dollar" style="width:100%; height: 185px;">
    </div>
  </header>
  <nav>
    <div class="navbar bg-base-100">
      <div class="navbar-start">
        <div class="dropdown">
        </div>
    </div>
  <div class="navbar-center hidden lg:flex text-white justify-evenly">
    <ul class="menu menu-horizontal px-1">
      <li class="text-xl hover:text-red-700"><a href="/">Home</a></li>
      <li class="text-xl hover:text-red-700"><a href="/episodes">Episodes</a></li>
      <li class="hover:text-red-700 text-xl">
          <a href="/about">About</a>
      </li>
      <li class="hover:text-red-700 text-xl"><a href="/blog"> Blog</a></li>
    </ul>
  </div>
  <div class="navbar-end justify-end">
    <a class="btn bg-red-700 text-white ">Subscribe</a>
  </div>
</div>
  </nav>
  <body>
    <slot />
  </body>
 <footer class="footer p-10 bg-base-200 text-base-content">
     <nav>
    <h6 class="footer-title">Services</h6> 
    <a class="link link-hover">Branding</a>
    <a class="link link-hover">Design</a>
    <a class="link link-hover">Marketing</a>
    <a class="link link-hover">Advertisement</a>
  </nav> 
  <nav>
    <h6 class="footer-title">Company</h6> 
    <a class="link link-hover">About us</a>
    <a class="link link-hover">Contact</a>
    <a class="link link-hover">Jobs</a>
    <a class="link link-hover">Press kit</a>
  </nav> 
  <nav>
    <h6 class="footer-title">Legal</h6> 
    <a class="link link-hover">Terms of use</a>
    <a class="link link-hover">Privacy policy</a>
    <a class="link link-hover">Cookie policy</a>
  </nav> 
  <form>
    <h6 class="footer-title">Newsletter</h6> 
    <fieldset class="form-control w-80">
      <label class="label">
        <span class="label-text">Enter your email address</span>
      </label> 
      <div class="join">
        <input type="text" placeholder="username@site.com" class="input input-bordered join-item" /> 
        <button class="btn bg-red-700 text-white hover:transparent join-item">Subscribe</button>
      </div>
    </fieldset>
  </form>
  </footer>
