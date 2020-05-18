
<TopAppBar {dense} {prominent} {variant} color='secondary'>
  <Row>
    <Section>
      <IconButton class="material-icons">menu</IconButton>
      <Title>Union y libertad</Title>
    </Section>
    <Section align="end" toolbar>
      <IconButton class="material-icons" aria-label="Download">file_download</IconButton>
      <IconButton class="material-icons" aria-label="Print this page">print</IconButton>
      <IconButton class="material-icons" aria-label="Bookmark this page">bookmark</IconButton>
    </Section>
  </Row>
</TopAppBar>
<div use:Adjust>
  <Home></Home>
</div>

<script>
  let dense = false;
  let prominent = true;
  let variant = 'standard';

  import TopAppBar, {Row, Section, Title, FixedAdjust, DenseFixedAdjust, ProminentFixedAdjust, ShortFixedAdjust} from '@smui/top-app-bar';
  import IconButton from '@smui/icon-button';
  import Home from './components/home.svelte';

  let Adjust = ProminentFixedAdjust;
</script>