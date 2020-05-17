<script>
  import Card, {
    Content,
    PrimaryAction,
    Media,
    MediaContent,
    Actions,
    ActionButtons,
    ActionIcons
  } from "@smui/card";
  import Button, { Label } from "@smui/button";
  import IconButton, { Icon } from "@smui/icon-button";
  import List, { Item, Text } from "@smui/list";
  import Grid from "svelte-grid-responsive";

  function doAction(action) {
    alert("You did an action: " + action);
  }
</script>

<section id="referentes" gutter="12">

<h1>Referentes</h1>
  <div>
    <h2>Tipito enojado</h2>
    <img src="https://yt3.ggpht.com/a/AATXAJx-k8hO9-6NQJB3qQw9KIB0Kn5hEtfhmuF6mA=s100-c-k-c0xffffffff-no-rj-mo" alt="tipito-logo"/>
    <p>
      Contenido del parrafo/ descripcion
    </p>
    <p>
      Segundo parrafo de la descripcion.
    </p>
  </div>
</section>
