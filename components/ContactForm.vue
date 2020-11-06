<template>
  <div id="contact-form-wrapper" class="flex justify-center items-center rounded">
    <form action="https://formspree.io/f/{form_id}" method="post">
      <!-- <label for="email"
             class="block font-bold">
             Your Email
      </label> -->
      <input id="email" class="mb-6 rounded font-bold"
             name="Email" type="email" placeholder="email">

      <!-- <label for="message"
             class="block font-bold">
             Message
      </label> -->

      <textarea id="message" class="mb-6 font-bold rounded" 
                name="message"
                placeholder="message">
      </textarea>

      <button type="submit"
              class="block font-bold rounded">
              Submit
      </button>
    </form>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  #contact-form-wrapper {
    margin: 0 auto;
    width: 50%;
    padding: 0px 4rem;
  }

  form {
    width: 100%;
  }

  textarea, input {
    width: 100%;
    padding: 0px 10px;
    background-color: rgb(34, 35, 35);
    border: 1px solid rgba(247, 250, 252, .1);
    font-size: 2rem;
    transition: all .2s ease-out;
  }

  input::placeholder {
    color: rgba(247, 250, 252, .2);
  }

  textarea::placeholder {
    color: rgba(247, 250, 252, .2);
  }

  input:focus {
    outline: none;
    border: 1px solid rgba(247, 250, 252, .2);
  }

  textarea:focus {
    outline: none;
    border: 1px solid rgba(247, 250, 252, .2);
  }

  input {
    height: 3.5rem;
  }

  textarea {
    height: 14rem;
    resize: none;
  }

  button {
    border: 1px solid rgba(247, 250, 252, .2);
    margin: 0 auto;
    padding: 10px;
    width: 30%;
    font-size: 2rem;
  }
</style>