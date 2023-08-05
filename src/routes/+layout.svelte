<script>
  import "../app.css";
  import LeftSidebar from "./leftSidebar.svelte";
  import RightSidebar from "./rightSidebar.svelte";
</script>

<main>
  <div class="grid grid-cols-1 sm:grid-cols-10">

    <!-- left side bar -->
    <div class="bg-blue-500 hidden sm:inline-block">
      <slot name="sidebar_left">
        <LeftSidebar/>
      </slot>
    </div>

    <!-- center -->
    <div class="bg-blue-500 col-span-6 row-span-1 z-50">
        <div class="bg-blue-600 sticky top-0 h-24 opacity-70 grid grid-cols-2 grid-flow-row">
          <div class="col-span-2 text-3xl">Home</div>
          <div class="text-center">For you</div>
          <div class="text-center">Following</div>
        </div>
        <slot />
    </div>

    <!-- left side bar -->
    <div class="bg-blue-500 hidden sm:block col-span-3">
      <slot name="sidebar_right">
        <RightSidebar />
      </slot>
    </div>
  </div>
</main>