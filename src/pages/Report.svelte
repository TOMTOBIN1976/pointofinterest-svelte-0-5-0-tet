<script>
  import poi from "/src/assets/point_of_interest.png";
  import DonationList from "../components/DonationList.svelte";
  import TitleBar from "../components/TitleBar.svelte";
  import MainNavigator from "../components/MainNavigator.svelte";
</script>

<div class="columns is-vcentered">
  <div class="column is-two-thirds">
    <TitleBar subTitle={"List"} title={"Points of Interest"}/>
  </div>
  <div class="column">
    <MainNavigator/>
  </div>
</div>

<div class="columns">
  <div class="column has-text-centered">
    <img alt="Homer" src={poi} width="300"/>
  </div>
  <div class="column box has-text-centered">
    <h1 class="title is-4">Points of Interest to date</h1>
    <DonationList/>
  </div>
</div>
