<script>
  import { Breadcrumbs } from 'sveltfy/src';

  const items = [
    { text: 'Dashboard', href: '/components/breadcrumbs/' },
    { text: 'Link 1', href: '/components/breadcrumbs/' },
    { text: 'Link 2', disabled: true },
  ];
</script>

<Breadcrumbs {items} />
<Breadcrumbs large {items} />
