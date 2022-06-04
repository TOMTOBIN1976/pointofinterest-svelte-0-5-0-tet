<script>
  import TitleBar from "../components/TitleBar.svelte";
  import MainNavigator from "../components/MainNavigator.svelte";
  import DonationsByCandidate from "../components/DonationsByCandidate.svelte";
  import DonationsMyMethod from "../components/DonationsMyMethod.svelte";
</script>

<div class="columns is-vcentered">
  <div class="column is-two-thirds">
    <TitleBar subTitle={"Points of Interest Analytics"} title={"Points of Interest Inc."}/>
  </div>
  <div class="column">
    <MainNavigator/>
  </div>
</div>

<div class="columns">
  <div class="column has-text-centered">
    <DonationsMyMethod/>
  </div>
  <div class="column has-text-centered">
    <DonationsByCandidate/>
  </div>
</div>