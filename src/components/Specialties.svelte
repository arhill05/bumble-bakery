<script>
  import Heading from './Heading.svelte';
</script>

<div class="specialties">
  <Heading text="Specialties" />
  <div class="specialties__list-container">
    <ul>
      <li>Weddings</li>
      <li>Birthdays</li>
      <li>Anniveraries</li>
      <li>Cupcakes</li>
      <li>Bridal Showers</li>
      <li>Small Batch</li>
    </ul>
  </div>
</div>

<style>
  .specialties {
    min-width: fit-content;
    justify-content: center;
  }

  .specialties__list-container ul {
    display: grid;
    gap: 25px;
    grid-template-columns: repeat(2, 1fr);
    justify-content: center;
    list-style: none;
    padding: 0;
    text-align: center;
    width: 100%;
  }

  .specialties__list-container ul li {
    font-weight: bold;
    font-size: 36px;
  }

  @media screen and (max-width: 760px) {
    .specialties {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 16px;
    }

    .specialties__list-container ul {
      grid-template-columns: repeat(1, 1fr);
    }
  }
</style>
