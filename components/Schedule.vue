<style lang="scss" scoped>
@import url("~/assets/scss/variables.scss");

#first-date {
  color: #108243;
}

#second-date {
  color: #0c826a;
}

#third-date {
  color: #04a09d;
}

.date {
  text-align: center;
  font-weight: 800;
  margin-bottom: 1.25em;
  font-size: 32px;
}

.event {
  padding: 0.5em;
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  align-items: center;
  border-radius: 8px;
}

.event:nth-child(odd) {
  background: rgba(255, 255, 255, 0.15);
}

.events-wrapper {
  padding: 20 30px;
  display: grid;
  grid: 1fr / 1fr 10px 1fr 10px 1fr;
  grid-gap: 10px;

  @media screen and (max-width: 768px /*break-l*/) {
    grid: 1fr 0px 1fr 0px 1fr / 1fr;
  }
}

.event-column {
  width: 100%;
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
}

.events {
  width: 100%;
}

.divider {
  height: 80%;
  background: black;
  align-self: center;
  border-radius: 6px;
}
</style>

<template>
  <div class="events-wrapper">
    <div class="event-column">
      <h3 id="first-date" class="date">Friday, Nov 2</h3>
      <div class="events">
        <div class="event">
          <div class="event-name">check-in</div>
          <div class="event-time">5:30p</div>
        </div>
        <div class="event">
          <div class="event-name">dinner</div>
          <div class="event-time">6:00p</div>
        </div>
        <div class="event">
          <div class="event-name">opening ceremony</div>
          <div class="event-time">8:00p</div>
        </div>
        <div class="event">
          <div class="event-name">hacking begins</div>
          <div class="event-time">10:00p</div>
        </div>
        <div class="event">
          <div class="event-name">pitch session</div>
          <div class="event-time">10:00p</div>
        </div>
        <div class="event">
          <div class="event-name">git tech talk</div>
          <div class="event-time">10:00p</div>
        </div>
        <div class="event">
          <div class="event-name">beginner switch session</div>
          <div class="event-time">10:30p</div>
        </div>
        <div class="event">
          <div class="event-name">beginner tech talks</div>
          <div class="event-time">11:00p</div>
        </div>
      </div>
    </div>
    <span class="divider" />
    <div class="event-column">
      <h3 id="second-date" class="date">Saturday, Nov 3</h3>
      <div class="events">
        <div class="event">
          <div class="event-name">midnight snack</div>
          <div class="event-time">12:00a</div>
        </div>
        <div class="event">
          <div class="event-name">intermediate tech talks</div>
          <div class="event-time">12:00a</div>
        </div>
        <div class="event">
          <div class="event-name">breakfast</div>
          <div class="event-time">8:00a</div>
        </div>
        <div class="event">
          <div class="event-name">advanced tech talks</div>
          <div class="event-time">9:00a</div>
        </div>
        <div class="event">
          <div class="event-name">lunch</div>
          <div class="event-time">12:00p</div>
        </div>
        <div class="event">
          <div class="event-name">dinner </div>
          <div class="event-time">5:30p</div>
        </div>
        <div class="event">
          <div class="event-name">wellness night</div>
          <div class="event-time">7:00p</div>
        </div>
        <div class="event">
          <div class="event-name">werewolf, hosted by MLH</div>
          <div class="event-time">9:00p</div>
        </div>
      </div>
    </div>
    <span class="divider" />
    <div class="event-column">
      <h3 id="third-date" class="date">Sunday, Nov 4</h3>
      <div class="events">
        <div class="event">
          <div class="event-name">midnight snack</div>
          <div class="event-time">12:00a</div>
        </div>
        <div class="event">
          <div class="event-name">breakfast</div>
          <div class="event-time">8:00a</div>
        </div>
        <div class="event">
          <div class="event-name">hacking ends</div>
          <div class="event-time">10:00a</div>
        </div>
        <div class="event">
          <div class="event-name">how to demo talk</div>
          <div class="event-time">10:00a</div>
        </div>
        <div class="event">
          <div class="event-name">lunch</div>
          <div class="event-time">11:00a</div>
        </div>
        <div class="event">
          <div class="event-name">project expo</div>
          <div class="event-time">11:30a</div>
        </div>
        <div class="event">
          <div class="event-name">closing ceremony</div>
          <div class="event-time">1:30p</div>
        </div>
        <div class="event">
          <div class="event-name">buses depart</div>
          <div class="event-time">3:30p</div>
        </div>
      </div>
    </div>
  </div>
</template>
