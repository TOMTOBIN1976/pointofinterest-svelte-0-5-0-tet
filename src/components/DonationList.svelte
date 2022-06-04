<script>
  import {getContext, onMount} from 'svelte'

  const donationService = getContext("DonationService");
  let donationList = [];

  onMount(async () => {
    donationList = await donationService.getDonations();
  });
</script>

<table class="table is-fullwidth">
  <thead>
    <th>Point of Interest</th>
    <th>Payment Options</th>
    <th>Coordinates</th>
    <th>Submitter</th>    
  </thead>
  <tbody>
    {#each donationList as donation}
      <tr>
        <td>
          {donation.amount}
        </td>
        <td>
          {donation.method}
        </td>
        <td>
          {donation.lng}, {donation.lat}
        </td>
        <td>
          {donation.donor.lastName},  {donation.donor.firstName}          
        </td>        
      </tr>
    {/each}
  </tbody>
</table>
