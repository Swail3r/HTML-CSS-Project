<template>
  <section class="contact-section">
    <h1>Contact Me</h1>

    <p>
      If you would like to get in touch with me, feel free to contact me.
    </p>

    <form
      action="https://formspree.io/f/xeedypao"
      method="POST"
    >
      <input
        type="hidden"
        name="_subject"
        value="New contact from portfolio"
      />

      <input
        type="hidden"
        name="_captcha"
        value="false"
      />

      <div>
        <label for="name">Name</label>
        <input
          type="text"
          id="name"
          name="name"
          placeholder="Your name"
          required
        />
      </div>

      <div>
        <label for="surname">Surname</label>
        <input
          type="text"
          id="surname"
          name="surname"
          placeholder="Your surname"
          required
        />
      </div>

      <div>
        <label for="phone">Phone Number</label>
        <input
          type="tel"
          id="phone"
          name="phone"
          placeholder="Your phone number"
          required
        />
      </div>

      <div>
        <label for="service">Service Needed</label>

        <select
          id="service"
          name="service"
        >
          <option value="">Select a service</option>
          <option value="web-design">Web Design</option>
          <option value="graphic-design">Graphic Design</option>
          <option value="consultation">Consultation</option>
        </select>
      </div>

      <div>
        <label for="email">Email</label>

        <input
          type="email"
          id="email"
          name="email"
          placeholder="Your email"
          required
        />
      </div>

      <div>
        <label for="message">Message</label>

        <textarea
          id="message"
          name="message"
          placeholder="Your message"
          required
        ></textarea>
      </div>

      <button type="submit">Send Message</button>
    </form>
  </section>
</template>