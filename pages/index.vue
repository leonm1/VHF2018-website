<template>
  <div class="main">
    <div class="top-background">
      <mlhbadge />
      <main class="landing-section">
        <img class="logo" alt="VandyHacks V" src="~assets/img/vh-logo-date.svg">
        <a ontouchstart="" class="apply-btn" href="https://apply.vandyhacks.org/login">Apply</a>
        <aside class="sponsor-prospectus">
          Interested in being a sponsor? <br> Check out our
          <a href="https://apply.vandyhacks.org/sponsorship">sponsorship prospectus</a>!
        </aside>
      </main>
      <section class="welcome-page">
        <img alt="Welcome" src="~assets/img/welcome.svg" class="heading-text">
        <content class="welcome">
          <p>Founded in the spring of 2015, VandyHacks was the first collegiate hackathon to call Nashville, Tennessee home. Now, we're proud to bring you VandyHacks V! From November 2-4, 2018, 450+ students from colleges and universities across the nation will gather at Vanderbilt University’s Engineering and Science Building for a weekend of collaboration, innovation, and entrepreneurship.</p>
          &nbsp;
          <p>For 36 hours, participants will work together to bring their ideas to life - and have lots of fun doing it! VandyHacks welcomes beginners, and we encourage all students to apply, regardless of their major or background.</p>
        </content>
      </section>
    </div>
    <section class="faq">
      <img alt="FAQ" src="~assets/img/faq.svg" class="heading-text">
      <section class="faq-column faq-left">
        <h3 class="faq-header">General</h3>
        <faqitem title="I have no idea how to code. Can I still attend?">
          Even more reason for you to come! We will be hosting beginners' workshops for you to get started, and our mentors can help you out along the way. We greatly encourage new hackers to attend, and no prior experience is necessary!
        </faqitem>
        <faqitem title="What if I've never been to a hackathon?">
          Not to worry! A few weeks before the event, we'll email you our hacker guide, which contains all the information you need to make the most out of your weekend. During the event, the VandyHacks Team will be around to help answer any questions. As always, feel free to email us at
          <a href="mailto:info@vandyhacks.org">info@vandyhacks.org</a> with any questions.
        </faqitem>
        <h3 class="faq-header">Applying</h3>
        <faqitem title="Who can apply?">
          Anyone who is 18 years or older and is currently enrolled in college or university with a valid student ID.
        </faqitem>
        <faqitem title="How does registration work?">
          Registration is currently open!
        </faqitem>
        <h3 class="faq-header">Travel</h3>
        <faqitem title="Will you be providing buses to schools?">
          Yes, we will be providing buses to Purdue University, University of Illinois at Urbana-Champaign, Georgia Institute of Technology, and University of Florida. We may also provide a bus at Illinois Institute of Technology for the Chicagoland area if we receive enough applications and RSVPs! If you reserve a seat on the bus (coming soon) and can get to the bus stop, you can get on!
        </faqitem>
        <faqitem title="How do I get there if I'm not near a bus stop?">
          We will be providing gas reimbursements for cars with 3+ hackers in them. Additionally, we may partially subsidize Greyhound and plane tickets. Contact us at
          <a href="mailto:travel@vandyhacks.org">travel@vandyhacks.org</a> if you have any questions.
        </faqitem>
        <faqitem title="Will there be parking available for attendees?">
          Yes! Attendees will be able to find parking at the 25th Avenue Garage, conveniently located next to Vanderbilt’s Engineering and Science Building. You can find it
          <a href="https://goo.gl/maps/qST6JAvvQAz">here</a>.
        </faqitem>
      </section>
      <section class="faq-column faq-right">
        <h3 class="faq-header">Event</h3>
        <faqitem title="What should I bring?">
          Be sure to bring your photo ID, laptop, phone, chargers, a change of clothes, toiletries, and any other devices you want to use. A government-issued ID is required to rent any hardware.
        </faqitem>
        <faqitem title="Where will I sleep?">
          We will have designated quiet rooms, so bring a blanket and pillow!
        </faqitem>
        <faqitem title="Is food provided?">
          Meals will be provided throughout the event, starting with Friday dinner and ending with lunch on Sunday. Snacks will also be provided periodically. Vegetarian and gluten-free options are available. Please indicate any allergies or dietary restrictions on your application.
        </faqitem>
        <faqitem title="How are teams formed? Do I need a team?">
          Teams are limited to four people. If you're applying with a team, we will review all of your team members' applications to determine admission. We will also have a pitch session where attendees can share their ideas and find potential teammates. However, teams are not required, so feel free to work individually.
        </faqitem>
        <faqitem title="Will there be other activities besides hacking?">
          Of course! This year, we've has planned a bunch of fun events for attendees to relax. Stay tuned for more info!
        </faqitem>
        <faqitem title="Do I need to stay the entire time?">
          Vanderbilt students are free to enter and leave the venue at all times. Students from other schools are asked to remain inside the venue throughout the entire event.
        </faqitem>
        <faqitem title="What if I’m interested in being a mentor?">
          Send us an email at
          <a href="mailto:mentor@vandyhacks.org">mentor@vandyhacks.org</a>.
        </faqitem>
        <h3 class="faq-header">Other</h3>
        <faqitem title="I have more questions!">
          Send us an email at
          <a href="mailto:info@vandyhacks.org">info@vandyhacks.org</a>! We'll be happy to answer!
        </faqitem>
      </section>
    </section>
    <section class="schedule">
      <img alt="Schedule" src="~assets/img/schedule.svg" class="heading-text">
      <schedule/>
    </section>
    <div class="footer">
      <section class="sponsors">
        <img alt="Sponsors" src="~assets/img/sponsors.svg" class="heading-text">
      </section>
      <sitefooter />
    </div>
  </div>
</template>

<script>
import MlhBadge from "~/components/MlhBadge.vue"
import Schedule from "~/components/Schedule.vue"
import FaqItem from "~/components/FaqItem.vue"
import Footer from "~/components/Footer.vue"
import Sponsors from "~/components/Sponsors.vue"

export default {
  components: {
    mlhbadge: MlhBadge,
    schedule: Schedule,
    faqitem: FaqItem,
    sitefooter: Footer,
    sponsors: Sponsors
  }
}
</script>

<style lang="scss">
@import "~/assets/scss/variables.scss";
body {
  width: 100%;
  overflow-x: hidden;
  color: white;
  font-size: 1.4em;
  font-family: "Sofia Pro";

  a {
    color: white;
  }

  @media screen and (max-width: $break-l) {
    font-size: 1em;
  }
}

.main {
  background: $background; /* Old browsers */
  background: linear-gradient(
    rgba(26, 23, 86, 1) 0%,
    rgba(26, 23, 86, 1) 50%,
    rgba(15, 11, 46, 1) 75%
  );
  display: grid;
  grid-auto-flow: row;
  grid-gap: 40px;
}

.heading-text {
  height: 10vh;
  width: 70vw;
  @media (min-width: $break-s) {
    width: 65vw;
  }
  @media (min-width: $break-sm) {
    width: 60vw;
  }
  @media (min-width: $break-m) {
    width: 55vw;
  }
  @media (min-width: $break-l) {
    width: 50vw;
  }
}

.top-background {
  background-image: url("~/assets/img/bg-top.svg");
  background-size: cover;
  background-position: right bottom;

  display: grid;
  grid-auto-flow: row;
  grid-gap: 40px;
}

.landing-section {
  padding: 20px 18px;
  padding-top: 10vh;
  height: 100vh;
  display: flex;
  flex-flow: column nowrap;
  justify-content: space-between;
  align-items: center;

  @media screen and (max-width: $break-m) {
    padding-top: 30%;
    display: grid;
    grid-auto-flow: row;
    grid-template-rows: auto;
    justify-content: center;
    align-items: center;

    aside {
      align-self: flex-end;
    }
  }
}

.logo {
  max-width: 95%;
  margin-bottom: 20px;

  width: 290px;
  @media (min-width: $break-s) {
    width: 320px;
  }
  @media (min-width: $break-m) {
    width: 390px;
  }
  @media (min-width: $break-l) {
    width: 495px;
  }
}

.apply-btn {
  color: $background;
  text-decoration: none;
  padding: 8px 40px;
  margin: 20px;
  background: $yellow-accent;
  border-radius: 4px;
  justify-self: center;
  transition: all 0.2s ease-out;
  &:hover {
    transform: scale(1.05);
    filter: brightness(150%);
    filter: contrast(150%);
  }

  @media screen and (max-width: 768px) {
    padding: 16px 80px;
    font-size: 1.6em;
  }
  @media screen and (max-width: 481px) {
    padding: 16px 40px;
  }
}

.sponsor-prospectus {
  align-self: flex-start;
  max-width: 50%;
  @media screen and (max-width: $break-m) {
    max-width: 100%;
  }
}

.welcome-page {
  padding-top: 16vh;
  padding: 18px;
  display: flex;
  flex-flow: column nowrap;
  justify-content: flex-end;
  p {
    margin-left: 60px;
  }

  @media screen and (min-width: 768px) and (orientation: landscape) {
    min-height: 100vh;

    .welcome {
      max-width: 60%;
    }
  }
}

.faq {
  background-image: url("~/assets/img/faq-background.svg");
  background-size: 100%;
  background-repeat: no-repeat;
  background-position: right bottom;
  padding: 0 18px;

  display: grid;
  grid:
    [row1-start] "header header" auto [row1-end]
    [row2-start] "blank left" auto [row2-end]
    [row3-start] "blank right" auto [row2-end]
    / 60px 1fr;

  & > img {
    grid-area: header;
  }
  .faq-left {
    grid-area: left;
  }
  .faq-right {
    grid-area: right;
  }

  @media screen and (min-width: 769px) and (orientation: landscape) {
    grid:
      [row1-start] "header header header header header" auto [row1-end]
      [row2-start] "break-left left break right break-right" 1fr [row2-end]
      / 60px 1fr 15px 1fr 60px;
  }
}

.schedule {
  padding: 0 18px;
  display: grid;
  grid:
    [row1-start] "header" auto [row1-end]
    [row2-start] "content" 1fr [row2-end]
    / 1fr;

  & > img {
    grid-area: header;
  }
}

.sponsors {
  background: rgba(15, 11, 46, 1) url(~assets/img/sponsors-background.svg)
    no-repeat;
  background-position: center center;
  background-size: cover;
  color: white;
}
</style>
