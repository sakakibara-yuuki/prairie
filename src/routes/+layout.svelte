<script>
  import "../app.css";
</script>


<header class="bg-yellow-500 fixed top-0 z-10 w-full">
  <p>hello</p>
</header>

<main class="mt-20">

<div class="grid grid-cols-1 sm:grid-cols-3">

  <!-- right side bar -->
  <div class="bg-blue-500 hidden sm:inline-block">
    <slot name="sidebar_left">
      <div class="sticky top-10 z-40">
        <h1>side bar left</h1>
        <h1>side bar left</h1>
        <h1>side bar left</h1>
      </div>
    </slot>
  </div>

  <!-- center -->
  <div class="bg-red-500">
    <slot />
  </div>

  <!-- left side bar -->
  <div class="bg-green-400 hidden sm:block">
    <slot name="sidebar_right">
      <div class="sticky top-10 z-40">
        <h1>side bar right</h1>
        <h1>side bar right</h1>
        <h1>side bar right</h1>
      </div>
    </slot>
  </div>
</div>
</main>