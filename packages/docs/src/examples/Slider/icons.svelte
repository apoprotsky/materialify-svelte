<script>
  import { Slider, Icon } from 'sveltfy/src';
  import { mdiMinus, mdiPlus } from '@mdi/js';
</script>

<Slider>
  <span slot="prepend-outer">
    <Icon path={mdiPlus} />
  </span>
  Icon
  <span slot="append-outer">
    <Icon path={mdiMinus} />
  </span>
</Slider>
