<script>
  import Button from '../lib/Button.svelte';
  import LastForm from '../lib/Form.svelte';
</script>


<!-- actual website content is here -->
<div class="min-h-screen p-8">
  <div class="flex justify-center gap-4">
    <LastForm class="">last.fm username</LastForm>
  </div>
</div>
<!-- website content ends -->



<style lang="postcss">
  @reference "tailwindcss";

  :global(html) {
    background-color: theme(--color-zinc-900);
  }
</style>
