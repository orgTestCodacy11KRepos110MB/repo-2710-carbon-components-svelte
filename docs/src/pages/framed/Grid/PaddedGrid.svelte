<script>
  import { Grid, Row, Column } from "carbon-components-svelte";
</script>

<div>Adding padding to Grid applies it to columns in all rows:</div>

<Grid padding>
  <Row>
    <Column>Column</Column>
    <Column>Column</Column>
    <Column>Column</Column>
    <Column>Column</Column>
  </Row>
</Grid>

<div>Adding padding to a Row only applies to its columns:</div>

<Grid>
  <Row padding>
    <Column>Column</Column>
    <Column>Column</Column>
    <Column>Column</Column>
    <Column>Column</Column>
  </Row>
  <Row>
    <Column>Column</Column>
    <Column>Column</Column>
    <Column>Column</Column>
    <Column>Column</Column>
  </Row>
</Grid>

<div>Adding padding to a specific column only applies it to the column:</div>

<Grid>
  <Row>
    <Column padding>Column</Column>
    <Column>Column</Column>
    <Column>Column</Column>
    <Column>Column</Column>
  </Row>
</Grid>

<style>
  div {
    margin-top: var(--cds-spacing-05);
    padding: var(--cds-spacing-05);
  }
</style>
