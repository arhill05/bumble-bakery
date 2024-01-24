<script>
  import Heading from './Heading.svelte';
</script>

<div class="contact" id="contact">
  <Heading text="Contact Us" />
  <div class="contact__info">
    <p><strong>Email:</strong> <em>Coming soon</em></p>
    <p><strong>Phone:</strong> <em>Coming soon</em></p>
  </div>
  <h2 class="contact__form-heading">Or send us a message here!</h2>
  <form name="contact" method="POST" data-netlify="true" class="contact__form">
    <p class="form-group">
      <label for="name">Your Name: </label>
      <input type="text" name="name" placeholder="John Doe" />
    </p>
    <p class="form-group">
      <label for="email">Your Email: </label>
      <input type="email" name="email" placeholder="john.doe@email.com" />
    </p>
    <p class="form-group">
      <label for="message"> What can we help you with? </label>
      <textarea name="message"></textarea>
    </p>
    <button class="action-button" type="submit">Send</button>
  </form>
</div>

<style>
  .contact__form-heading {
    color: var(--brand-color);
  }

  .contact__info,
  .contact__form {
    font-size: 24px;
  }

  .contact__form label {
    font-weight: bold;
  }

  input,
  textarea {
    border: none;
    border-bottom: 2px solid var(--brand-color);
  }

  .form-group {
    display: flex;
    flex-direction: column;
  }

  .action-button {
    background-color: var(--brand-color);
    border: none;
    padding: 12px 24px;
    border-radius: 4px;
    cursor: pointer;
    box-shadow: 4px 4px 0 0 rgba(0, 0, 0, 0.2);
  }

  .action-button:hover {
    filter: brightness(90%);
  }

  .action-button:active {
    box-shadow: none;
    filter: brightness(87%);
  }

  .contact {
    padding-bottom: 32px;
  }

  @media screen and (max-width: 760px) {
    .contact {
      padding: 16px;
    }

    .contact {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 16px;
    }
  }
</style>
