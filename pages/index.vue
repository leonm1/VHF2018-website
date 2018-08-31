<template>
  <section class="parallax">
    <div class="parallax-group">
      <div class="parallax-layer base">
        <mlhbadge></mlhbadge>
      </div>
      <div class="parallax-layer deep">
        <div class="logo">
          <img alt="VandyHacks V" src="~assets/img/vh-logo-date.svg"/>
          <div class="actions">
            <a ontouchstart="" class="apply-btn" href="https://vandyhacksiv.devpost.com/submissions">Apply</a>
          </div>
        </div>
      </div>
    </div>
    <div class="parallax-layer base page-content">
      <div class="description feature-block">
        <div class="text-contents">
          <img alt="Welcome" src="~assets/img/welcome.svg" class="heading-text"/>
          <p>Founded in the spring of 2015, VandyHacks was the first collegiate hackathon to call Nashville,
            Tennessee home. Now, we're proud to bring you VandyHacks V! From November 2-4, 2018, 450+
            students from colleges and universities across the nation will gather at Vanderbilt
            University’s Engineering and Science Building for a weekend of collaboration, innovation,
            and entrepreneurship.</p>
          &nbsp;
          <p>For 36 hours, participants will work together to bring their ideas to life - and have lots
            of fun doing it! VandyHacks welcomes beginners, and we encourage all students to apply,
            regardless of their major or background.</p>
        </div>
      </div>
      <div class="faq feature-block">
        <div class="text-contents">
          <img alt="FAQ" src="~assets/img/faq.svg" class="heading-text"/>
          <div class="row">
            <div class="col-sm-6 col-md-6 faq-col">
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
            </div>
            <div class="col-sm-6 col-md-6 faq-col">
              <h3 class="faq-header">Event</h3>
              <faqitem title="What should I bring?">
                Be sure to bring your photo ID, laptop, phone, chargers, a change of clothes, toiletries, and any other devices you want to use. A government-issued ID is required to rent any hardware.
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
            </div>
          </div>
        </div>
      </div>
      <div class="schedule feature-block">
        <div class="text-contents">
          <img alt="Schedule" src="~assets/img/schedule.svg" class="heading-text"/>
          <schedule/>
        </div>
      </div>
      <div class="sponsors feature-block">
        <div class="text-contents">
          <img alt="Sponsors" src="~assets/img/sponsors.svg" class="heading-text"/>
          <sponsors/> &nbsp;
        </div>
      </div>
      <sitefooter />
    </div>
  </section>
</template>

<script>
import MlhBadge from '~/components/MlhBadge.vue'
import Schedule from '~/components/Schedule.vue'
import FaqItem from '~/components/FaqItem.vue'
import Sponsors from '~/components/Sponsors.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    mlhbadge: MlhBadge,
    schedule: Schedule,
    faqitem: FaqItem,
    sponsors: Sponsors,
    sitefooter: Footer
  },
  mounted() {
    if (process.browser) {
      const xhr = new XMLHttpRequest()
      xhr.open('GET', 'https://apply.vandyhacks.org/wakemydyno.txt', true)
      xhr.send()
    }
  }
}
</script>

<style lang="scss">
@import '~assets/scss/parallax.scss';
@import '~assets/scss/breakpoints.scss';

html {
  background: #1A1756;  /* fallback for old browsers */
}

// There are offset issues on Chrome desktop, most noticeable at extremely low widths
// Won't fix, the offsets are fine on mobile where they matter - Yunyu
.logo {
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  margin: 16vh auto 0; // Responsiveness
  width: 290px;

  @media (min-width: $break-s) {
    width: 320px;
  }

  @media (min-width: $break-sm) {
    width: 390px;
  }

  @media (min-width: $break-m) {
    width: 495px;
    margin-top: 14.5vh;
  }

  @media (min-width: $break-l) {
    width: 635px;
  }
}

.actions {
  text-align: center;
  margin-top: 40px;

  @media (min-width: $break-m) {
    margin-top: 45px;
  }

  @media (min-width: $break-l) {
    margin-top: 50px;
  }
}

.apply-btn {
  $btn-bg: #222a53;
  $btn-font-size: 14.5px;
  $btn-padding-v: 15.75px;
  $btn-padding-h: 1.5 * $btn-padding-v;

  color: white;
  background-color: $btn-bg;
  border-radius: 3px;
  text-decoration: none;
  padding: $btn-padding-v $btn-padding-h;
  font-size: $btn-font-size;
  font-weight: bold;
  transition: all 0.15s linear;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
  cursor: pointer;

  &:hover,
  &:focus {
    background-color: #394574;
  }

  &:active {
    background-color: darken($btn-bg, 10%);
  }
}

.page-content {
  top: 100%;
  background: #fff;
}

.feature-block {
  background: #fff;
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

.text-contents {
  font-family: 'Sofia Pro';
  max-width: 768px;
  padding: 36px;
  line-height: 1.5em;

  @media (min-width: $break-l) {
    padding: 60px;
  }

  h1 {
    text-align: left;
    @media (min-width: $break-l) {
      font-size: 36px;
    }
  }
}

// Content sections
.description {
  background: #131349;
  color: white;
}

.schedule {
  background: #0F0B2E;
  color: white;
}

.faq {
  background: #131349;
  color: white;

  @media (min-width: $break-l) {
    background: #131349 url(~assets/img/faq-background.svg) no-repeat;
    background-position: center bottom;
    background-size: 110% 50%;
  }
}

.faq {
  text-align: center;

  a {
    color: #d0d3e1;
  }
}

.faq,
.schedule {
  .text-contents {
    text-align: left; // padding-bottom: 15px;
    max-width: 100%;
  }
}

.faq-header {
  text-decoration: underline;
  font-weight: normal;
  margin-top: 20px;
}

.faq-desk {
  max-width: 500px;
  margin-left: 30px;
  margin-right: 30px;
}

.faq-col:last-child {
  width: 100%;

  @media only screen and (min-width: 48em) {
    width: auto;
    padding-left: 20px;
  }

  @media only screen and (min-width: 64em) {
    padding-left: 30px;
  }
}

.sponsor-info {
  max-width: 1200px;
  text-align: center;
  font-weight: normal;
  font-size: 1.14em;
}

.sponsors {
  background: #131349 url(~assets/img/sponsors-background.svg) no-repeat;
  background-position: center center;
  background-size: cover;
  color: white;
}
</style>
