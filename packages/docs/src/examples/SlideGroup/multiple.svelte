<script>
  import { SlideGroup, SlideItem, Button } from 'sveltfy/src';
</script>

<SlideGroup multiple>
  {#each Array(10) as _, i}
    <SlideItem let:active>
      <Button class="mr-2 ml-2 {active ? 'primary-color' : ''}">Button {i + 1}</Button>
    </SlideItem>
  {/each}
</SlideGroup>
