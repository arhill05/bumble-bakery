<script>
  import Image from './Image.svelte';
  import Heading from './Heading.svelte';
</script>

<div class="media">
  <Heading text="Work" />
  <div class="media__photos-container">
    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1696859120/bumble-bakery/lover-cake.jpg"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1696859120/bumble-bakery/lover-cake.jpg"
      alt="Lover cake"
    />

    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1696859120/bumble-bakery/sugar-cookies-1.jpg"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1696859120/bumble-bakery/sugar-cookies-1.jpg"
      alt="Sugar cookies"
    />

    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1696859120/bumble-bakery/sugar-cookies-2.jpg?"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1696859120/bumble-bakery/sugar-cookies-2.jpg"
      alt="More sugar cookies"
    />

    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1696859120/bumble-bakery/sugar-cookies-3.jpg?"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1696859120/bumble-bakery/sugar-cookies-3.jpg"
      alt="Even more sugar cookies"
    />

    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1696859120/bumble-bakery/taylor-swift-cupcakes-1.jpg"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1696859120/bumble-bakery/taylor-swift-cupcakes-1.jpg"
      alt="Taylor Swift cupcakes"
    />

    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1696859120/bumble-bakery/taylor-swift-cupcakes-2.jpg?"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1696859120/bumble-bakery/taylor-swift-cupcakes-2.jpg"
      alt="More Taylor Swift cupcakes"
    />

    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1696859120/bumble-bakery/bee-cake-1.jpg"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1696859120/bumble-bakery/bee-cake-1.jpg"
      alt="Bee cake"
    />

    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1706064137/bumble-bakery/apple-cupcake.jpg"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1706064137/bumble-bakery/apple-cupcake.jpg"
      alt="Apple caramel cupcakes with an apple slice garnish"
    />

    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1706064327/bumble-bakery/sprinkle-happy-birthday.jpg"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1706064327/bumble-bakery/sprinkle-happy-birthday.jpg"
      alt="Birthday cake decorated with sprinkles and a happy birthday sign"
    />

    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1706064932/bumble-bakery/minnie-mouse-baby-shower-cupcake.jpg"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1706064932/bumble-bakery/minnie-mouse-baby-shower-cupcake.jpg"
      alt="Minnie Mouse themed baby shower cupcakes with pink frosting and mini Oreos as ears"
    />

    <Image
      fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1706064326/bumble-bakery/50_anniversary.jpg"
      smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1706064326/bumble-bakery/50_anniversary.jpg"
      alt="50th anniversary cake"
    />
  </div>
</div>

<style>
  .media {
    min-width: fit-content;
    justify-content: center;
  }

  .media__photos-container {
    display: grid;
    text-align: center;
    grid-template-columns: repeat(2, 1fr);
    gap: 25px;
    width: 100%;
  }

  :global(.media a:last-of-type) {
    grid-column: span 2;
    justify-self: center;
  }

  @media screen and (max-width: 760px) {
    .media {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 16px;
    }

    .media__photos-container {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    :global(.media a:last-of-type) {
      grid-column: unset;
      justify-self: unset;
    }
  }
</style>
