<script>
  import { Subheader, ListItem, Icon } from 'sveltfy/src';
  import { mdiLabel } from '@mdi/js';
</script>

<div class="ml-auto mr-auto elevation-2 pa-2" style="width:400px">
  <Subheader inset>Subheader</Subheader>
  {#each Array(3) as _, i}
    <ListItem>
      <span slot="prepend">
        <Icon path={mdiLabel} />
      </span>
      List Item
      {i + 1}
    </ListItem>
  {/each}
</div>
