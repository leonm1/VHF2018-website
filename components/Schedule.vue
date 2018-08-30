<style scoped>
.sched-col {
    flex: 1;
    margin: 20px 1.5em 0;
}

@media (max-width: 1023px) {
    .sched-col {
        flex: 0 0 100%;
        margin-left: 0;
        margin-right: 0;
        margin-bottom: 1.25em;
    }
}

@media (min-width: 1024px) and (max-width: 1279px) {
    .sched-col {
        margin: 20px 1em 0;
    }
}

.sched-col:first-child {
    margin-left: 0;
}

.sched-col:last-child {
    margin-right: 0;
}

.date {
    /*text-decoration: underline;*/
    text-align: center;
    font-weight: 800;
    margin-bottom: 1.25em;
    font-size: 1.5em
}

.first-date {
    color: #108243;
}

.second-date {
    color: #0C826A;
}

.third-date {
    color: #04A09D;
}

.event {
    padding: .75em;
}

.event:nth-child(even):last-child {
    padding-bottom: .5em;
}

.event:nth-child(odd) {
    background: rgba(255, 255, 255, 0.15);
}

.event-name,
.event-time {
    display: inline-block;
}

.event-name {
    font-weight: bold;
}

.event-time {
    float: right;
}
</style>

<template>
    <div class="row">
        <div class="sched-col">
            <h3 class="date first-date">Friday, Nov 2</h3>
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
        <div class="sched-col">
            <h3 class="date second-date">Saturday, Nov 3</h3>
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
        <div class="sched-col">
            <h3 class="date third-date">Sunday, Nov 4</h3>
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
