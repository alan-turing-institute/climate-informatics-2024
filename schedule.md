---
layout: page
title: Schedule
---


<script>
const ALL_DAYS = ["04-22", "04-23", "04-24"];

function setupActiveDayTab(activeDay) {
    /* First, remove the "active" classname for all tabs */
    ALL_DAYS.forEach(day => {
        let divDay = document.getElementById(`day-${day}`);
        divDay.className = divDay.className.replace("active", "");
    });
    
    /* Then add it to the appropriate day */
    let divDay = document.getElementById(`day-${activeDay}`);
    divDay.className = `${divDay.className} active`;
}

function setupActiveDaySchedule(activeDay) {
    /* First, hide all the schedule blocks */
    ALL_DAYS.forEach(day => {
        let divDay = document.getElementById(`schedule-${day}`);
        divDay.className = divDay.className.replace("active", "");
    });
    
    /* Then display:block to show the appropriate one */
    let divDay = document.getElementById(`schedule-${activeDay}`);
    divDay.className = `${divDay.className} active`;
}

function showScheduleForDay(day) {
    setupActiveDayTab(day);
    setupActiveDaySchedule(day);
}
</script>


<div class="schedule-days">
  <div id="day-04-22" class="schedule-day active" onclick="showScheduleForDay('04-22')">22nd April</div>
  <div id="day-04-23" class="schedule-day" onclick="showScheduleForDay('04-23')">23rd April</div>
  <div id="day-04-24" class="schedule-day" onclick="showScheduleForDay('04-24')">24th April</div>
</div>

<h5 style="text-align: center;">
<mark>Coming soon: Full schedule information will be shared soon!</mark>

<p>
<b><i>CI2024 will take place 22nd-24th April 2024, in <a href="https://bmahouse.org.uk">BMA House</a>, London, UK.</i></b> 
<br><br><b>Add a "save the date" to your calendar here:</b> <a title="Add to Calendar" class="addeventatc" data-id="rw19409406" href="https://www.addevent.com/event/rw19409406" target="_blank">Add to Calendar</a> <script type="text/javascript" src="https://cdn.addevent.com/libs/atc/1.6.1/atc.min.js" async defer></script>
</p>

<!-- <p>UTC</p> -->
</h5>

<div id="schedule-04-22" class="schedule-block">
    <h4>Monday 22nd April 2024</h4>

    <div class="schedule-content">
        <table class="osr-schedule">
            <tr>
                <td>GMT-4</td>
                <td>TRAINING AND HACKATHON</td>
            </tr>
            <tr>
                <td>8:00-9:00</td>
                <td>
                    <div><a href="" target="_blank">Training 1:</a> Abstract</div>
                    <div><a href="https://www.crowdcast.io/e/panel-1-telehealth" target="_blank">Join on Zoom</a></div>
                </td>
            </tr>
            <tr>
                <td>10:30-11:30</td>
                <td>
                    <div><a href="" target="_blank">Training 2:</a> Abstract</div>
                    <div><a href="https://www.crowdcast.io/e/panel-1-telehealth" target="_blank">Join on Zoom</a></div>
                </td>
            </tr>
            <tr>
                <td>11:30-12:15</td>
                <td>
                    <div><a href="" target="_blank">Lunch:</a> Abstract</div>
                    <div><a href="https://www.crowdcast.io/e/panel-1-telehealth" target="_blank">Join on Zoom</a></div>
                </td>
            </tr>
            <tr>
                <td>14:15-15:30</td>
                <td>
                    <div><a href="" target="_blank">Hack 1:</a> Abstract</div>
                    <div><a href="https://www.crowdcast.io/e/panel-1-telehealth" target="_blank">Join on Zoom</a></div>
                </td>
            </tr>
            <tr>
                <td>16:45-17:30</td>
                <td>
                    <div><a href="" target="_blank">Hack 2:</a> Abstract</div>
                    <div><a href="https://www.crowdcast.io/e/panel-1-telehealth" target="_blank">Join on Zoom</a></div>
                </td>
            </tr>
        </table>
    </div>
</div>

<div id="schedule-04-23" class="schedule-block">
    <h4>Tuesday 23rd April 2024</h4>

    <div class="schedule-content">
        <table class="osr-schedule">
            <tr>
                <td>GMT-4</td>
                <td>OPEN SCIENCE ROOM</td>
            </tr>
            <tr>
                <td>8:00-9:00</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/panel/" target="_blank">Panel:</a> Standardization of Code (tips)</div>
                    <div><a href="https://www.crowdcast.io/e/panel-3-standardization" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>10:30-11:30</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/emergent/" target="_blank">Emergent Session:</a> Developing a community-driven standard file format for brain tractography</div>
                    <div><a href="https://www.crowdcast.io/e/osr-2023-emergent-2" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>12:15-13:00</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/tabletalk/" target="_blank">Table Topic Discussion:</a> Standardization of Code</div>
                    <div><a href="https://www.crowdcast.io/e/osr-table-standardization" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>14:45-15:45</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/emergent/" target="_blank">Emergent Session:</a> Discuss ideas for longitudinal simulated datasets for interplay of brain, behavior, and cognition</div>
                    <div><a href="https://www.crowdcast.io/e/osr-2023-emergent-3" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
        </table>
    </div>
</div>

<div id="schedule-04-24" class="schedule-block">
    <h4>Wednesday 24th April 2024</h4>

    <div class="schedule-content">
        <table class="osr-schedule">
            <tr>
                <td>GMT-4</td>
                <td>OPEN SCIENCE ROOM</td>
            </tr>
            <tr>
                <td>8:00-9:00</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/emergent/" target="_blank">Emergent Session:</a> Enabling federated analysis on large datasets with COINSTAC Vaults</div>
                    <div><a href="https://www.crowdcast.io/e/osr-2023-emergent-4" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>8:00-9:15</td>
                <td>
                    <div>Morning Symposia: Open Science - sustainability through success stories</div>
                </td>
            </tr>
            <tr>
                <td>10:30-11:30</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/panel/" target="_blank">Panel:</a> Open Data Governance and Infrastructure</div>
                    <div><a href="https://www.crowdcast.io/e/panel-4-data-governance" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>11:45-12:45</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/tabletalk/" target="_blank">Table Topic Discussion:</a> Open Data Governance and Infrastructure - Sharable Resources in Neuroimaging</div>
                    <div><a href="https://www.crowdcast.io/e/osr-table-data-governance" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>14:00-14:30</td>
                <td>
                    <div>Off Schedule Session: Mathworks</div>
                    <div><a href="https://www.crowdcast.io/c/osr-mathworks" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            
            <tr>
                <td>14:45-16:15</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/emergent/" target="_blank">Emergent Session:</a> Physiopy open meeting: physiology community practices + Challenges for small collaborative software projects</div>
                    <div><a href="https://www.crowdcast.io/e/osr-2023-emergent-5" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
        </table>
    </div>
</div>

<div class="schedule-leave-space-before-footer">
</div>

<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src='https://plugins.eventable.com/eventable.js';fjs.parentNode.insertBefore(js,fjs);}}(document,'script', 'eventable-script');</script>

