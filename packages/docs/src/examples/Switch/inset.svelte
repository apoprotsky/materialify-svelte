<script>
  import { Switch } from 'sveltfy/src';

  const values = [false, true];
</script>

<Switch bind:checked={values[0]} inset>Inset {values[0]}</Switch>
<Switch bind:checked={values[1]} inset>Inset {values[1]}</Switch>
