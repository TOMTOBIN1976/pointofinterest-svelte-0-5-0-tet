<script>
  import poi from "/src/assets/point_of_interest.png";
  import WelcomeNavigator from "../components/WelcomeNavigator.svelte";
  import TitleBar from "../components/TitleBar.svelte";
  import {getContext} from "svelte";

  const donationService = getContext("DonationService");
  donationService.logout();
</script>

<div class="columns is-vcentered">
  <div class="column is-two-thirds">
    <TitleBar subTitle={"Sign up or Log in"} title={"Donation Services Inc."}/>
  </div>
  <div class="column">
    <WelcomeNavigator/>
  </div>
</div>

<div class="columns is-vcentered content">
  <div class="column has-text-centered">
    <img alt="homer" src="{poi}" width="300">
  </div>
  <div class="column">
    <h1 class="title">Points of Interest</h1>
    <p>Add your points of Interest.</p>
  </div>
</div>

