<script>
  import { Button, Overlay } from 'sveltfy/src';

  let active = false;
</script>

<div class="text-center">
  <Button
    class="red white-text"
    on:click={() => {
      active = true;
    }}>
    Show Overlay
  </Button>
</div>

<Overlay
  {active}
  on:click={() => {
    active = false;
  }} />
