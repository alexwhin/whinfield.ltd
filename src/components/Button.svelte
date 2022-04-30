<script>
  import Fa from "svelte-fa";

  export let href = "javascript:void(0);";
  export let target = "_blank";

  export /**
   * @type {import("@fortawesome/fontawesome-common-types").IconDefinition}
   */
  let icon;
</script>

<a
  class="rounded-xl bg-black text-stone-300 inline-block px-3 py-1 transition-all hover:text-black hover:bg-transparent border-solid border-2 border-black"
  {href}
  {target}
  {...$$restProps}
>
  <span class="flex items-center justify-center">
    {#if icon}
      <Fa class="mr-2" {icon} />
    {/if}
    <slot />
  </span>
</a>
