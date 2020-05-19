<script>
  let dense = false;
  let prominent = true;
  let variant = "standard";

  let isOpen = false;

  function handleUpdate(event) {
    isOpen = event.detail.isOpen;
  }

  import TopAppBar, {
    Row,
    Section,
    Title,
    FixedAdjust,
    DenseFixedAdjust,
    ProminentFixedAdjust,
    ShortFixedAdjust
  } from "@smui/top-app-bar";
  import IconButton from "@smui/icon-button";
  import Home from "./components/home.svelte";
  import {
    Collapse,
    Navbar,
    NavbarToggler,
    NavbarBrand,
    Nav,
    NavItem,
    NavLink,
    UncontrolledDropdown,
    DropdownToggle,
    DropdownMenu,
    DropdownItem
  } from "sveltestrap";

  let Adjust = ProminentFixedAdjust;
</script>

<TopAppBar {dense} {prominent} {variant} color="secondary">
  <Row>
    <Section>
      <!--<IconButton class="material-icons">menu</IconButton>-->
      <Title>Union y libertad</Title>
    </Section>
    <Section align="end" toolbar>
      <Nav>
        <NavItem>
          <NavLink href="#">Link</NavLink>
        </NavItem>
        <NavItem>
          <NavLink href="#">Link</NavLink>
        </NavItem>
        <NavItem>
          <NavLink href="#">Another Link</NavLink>
        </NavItem>
        <NavItem>
          <NavLink disabled href="#">Disabled Link</NavLink>
        </NavItem>
      </Nav>
    </Section>
  </Row>
</TopAppBar>
<div use:Adjust>
  <Home />
</div>
