<script>
  import Image from './Image.svelte';
  import Heading from './Heading.svelte';
</script>

<div class="about">
  <Heading text="About" />
  <div class="about__content">
    <div class="about__content-image">
      <Image
        fullSizeSrc="https://res.cloudinary.com/df3ikytgy/image/upload/v1706066161/bumble-bakery/julie_headshot.jpg"
        smallSrc="https://res.cloudinary.com/df3ikytgy/image/upload/w_425/q_auto/f_auto/v1706066161/bumble-bakery/julie_headshot.jpg"
        alt="Julie's headshot"
      />
    </div>
    <div class="about__content-text">
      <p>
        Hey there, I'm Julie! I'm a special education teacher in Oldham County, Kentucky, and I'm
        the face behind Bumble Bakery.
      </p>

      <p>
        Baking has always been a passion of mine. When I finish a day of teaching, I often head home
        to my kitchen, blast some Taylor Swift, dance with my Corgi Lucy, and bake some delicious
        treats. I'd love to share them with you, so fill out the form below and let's work together
        to create something delicious!
      </p>
    </div>
  </div>
</div>

<style>
  .about {
    margin: 0 auto;
    max-width: 1200px;
    padding: 0 1rem;
  }

  .about__heading {
    font-family: var(--font-family-heading);
    font-size: 2.5rem;
    margin-bottom: 1rem;
    text-align: center;
  }

  .about__content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin: 0 auto;
    max-width: 1200px;
  }

  .about__content-image {
    margin: 0 auto;
    max-width: 425px;
  }

  .about__content-text {
    font-size: 1.25rem;
    line-height: 1.5;
    margin: 0 auto;
    max-width: 600px;
  }

  .about__content-text__brand-emphasis {
    color: var(--brand-color);
    font-family: var(--font-family-heading);
    font-size: 1.5rem;
    font-weight: 700;
  }

  @media (min-width: 768px) {
    .about__content {
      flex-direction: row;
    }

    .about__content-image {
      margin-right: 2rem;
    }
  }
</style>
