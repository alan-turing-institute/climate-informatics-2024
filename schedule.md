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
  <div id="day-04-22" class="schedule-day active" onclick="showScheduleForDay('04-22')">22 April 2024</div>
  <div id="day-04-23" class="schedule-day" onclick="showScheduleForDay('04-23')">23 April 2024</div>
  <div id="day-04-24" class="schedule-day" onclick="showScheduleForDay('04-24')">24 April 2024</div>
</div>

<h5 style="text-align: center;" id="anchor_top">
<!-- <mark>Coming soon: Full schedule information will be shared soon!</mark> -->

<p>
<b><i>CI2024 will take place 22-24 April 2024, in <a href="https://bmahouse.org.uk">BMA House</a>, London, UK and online.</i></b> 
<!-- <br><br><b>Add a "save the date" to your calendar here:</b> <a title="Add to Calendar" class="addeventatc" data-id="rw19409406" href="https://www.addevent.com/event/rw19409406" target="_blank">Add to Calendar</a> <script type="text/javascript" src="https://cdn.addevent.com/libs/atc/1.6.1/atc.min.js" async defer></script> -->
<br><br>Please visit <a href="https://www.eventsforce.net/turingevents/frontend/reg/thome.csp?pageID=146256&eventID=358&traceRedir=2" target="_blank">The Alan Turing Institute event page</a> to register by 17 April 2024.

</p>
</h5>

<div id="schedule-04-22" class="schedule-block">
    <h4>Monday 22 April 2024</h4>

    <div class="schedule-content">
        <table class="osr-schedule">
            <tr>
                <td>UTC+1</td>
                <td>DAY 1</td>
            </tr>
            <tr>
                <td>09:30-10:30</td>
                <td>
                    <div><a href="" target="_blank"></a> Registration and networking with welcome refreshments</div>
                </td>
            </tr>
            <tr>
                <td>10:30-11:00</td>
                <td>
                    <div>Welcome remarks <a href="../team#mcs-and-session-chairs">(Scott Hosking)</a></div>
                </td>
            </tr>
            <tr>
                <td>11:00-12:00</td>
                <td>
                    <div><a href="../speakers/tamsin_edwards.html">How uncertain is future sea level rise? (Tamsin Edwards)</a></div>
                </td>
            </tr>
            <tr>
                <td>12:00-12:30</td>
                <td>
                    <div>Morning break with refreshments</div>
                </td>
            </tr>
            <tr>
                <td>12:30-13:35</td>
                <td>
                    <div>On Societal-relevant Applications (Chair <a href="../team#mcs-and-session-chairs">Alden Conner</a>)</div>
                    <div>
                    <ol>
                    <li><a href="../speakers/isabelle_tingzon.html">Mapping Housing Stock Characteristics from Drone Images for Climate Resilience in the CaribbeanAnnotations via NIDM-Terms Fosters Improved Search of OpenNeuro Datasets (Isabelle Tingzon)</a></li>
                    <li><a href="../speakers/paul_harris.html">Envisioning Digital Twins for Instrumented Farms of the Future (Paul Harris)</a></li>
                    <li><a href="../speakers/arjun_biswas.html">Using a large language model to create a chatbot companion for a major climate report (Arjun Biswas)</a></li>
                    </ol>
                    </div>
                </td>
            </tr>
            <tr>
                <td>13:35-14:50</td>
                <td>
                    <div>Lunch</div>
                </td>
            </tr>
            <tr>
                <td>16:45-17:30</td>
                <td>
                    <div>On Hydrology modelling (Chair <a href="../team#mcs-and-session-chairs">Kenza Tazi</a>)</div>
                    <div>
                    <ol>
                    <li><a href="../speakers/peter_miersch.html"> Sensitivity analysis of causal discovery on simulated river flood data using non-linear conditional independence testing (Peter Miersch)</a></li>
                    <li><a href="../speakers/robert_rouse.html">Gaussian & Neural Processes in Hydrology (Robert Rouse)</a></li>
                    <li><a href="../speakers/james_briant.html">Hybrid climate simulation including machine-learnt subgrid variability from kilometre-scale weather simulation (James Briant)</a></li>
                    </ol>
                    </div>                
                </td>
            </tr>
            <tr>
                <td>15:55-16:25</td>
                <td>
                    <div>Afternoon break with refreshments</div>
                </td>
            </tr>
            <tr>
                <td>16:25-17:25</td>
                <td>
                    <div><a href="../speakers/ilan_price.html">Progress and challenges in ensemble weather forecasting with machine learning (Ilan Price)</a></div>
                </td>
            </tr>
            <tr>
                <td>17:25-17:35</td>
                <td>
                    <div>Closing remarks for Day 1 <a href="../team#mcs-and-session-chairs">(Scott Hosking)</a></div>
                </td>
            </tr>
            <tr>
                <td>18:15-onwards</td>
                <td>
                    <div>“Climate Quizformatics” at Impact Hub, Euston (in-person attendees only, Hosts (<a href="../team#mcs-and-session-chairs">Katy Thompson</a> and <a href="../team#mcs-and-session-chairs">Andrew McDonald</a>)</div>
                </td>
            </tr>
        </table>
    </div>
    <h5><a href="#anchor_top">Jump to top of schedule</a></h5>
</div>

<div id="schedule-04-23" class="schedule-block">
    <h4>Tuesday 23 April 2024</h4>

    <div class="schedule-content">
        <table class="osr-schedule">
            <tr>
                <td>UTC+1</td>
                <td>DAY 2</td>
            </tr>
            <tr>
                <td>09:00-09:30</td>
                <td>
                    <div>Registration with welcome refreshments</div>
                </td>
            </tr>
            <tr>
                <td>09:30-09:35</td>
                <td>
                    <div>Welcome back (<a href="../team#mcs-and-session-chairs">Orlando Timmerman</a> and <a href="../team#mcs-and-session-chairs">Andrew McDonald</a>)</div>
                </td>
            </tr>
            <tr>
                <td>09:35-10:35</td>
                <td>
                    <div><a href="../speakers/peter_dueben.html">The digital revolution of Earth system modelling (Peter Dueben)</a></div>
                </td>
            </tr>
            <tr>
                <td>10:40-11:45</td>
                <td>
                    <div>On Weather & climate modeling (Chair <a href="../team#mcs-and-session-chairs">Douglas Rao</a>)</div>
                    <div>
                    <ol>
                    <li><a href="../speakers/oscar_key.html"> Scalable Data Assimilation with Message Passing (Oscar Key)</a></li>
                    <li><a href="../speakers/doug_mcneall.html">Will a climate simulation run? (Doug McNeall)</a></li>
                    <li><a href="../speakers/hannah_christensen.html">Machine Learning for Stochastic Parametrisation (Hannah Christensen)</a></li>
                    </ol>
                    </div>                
                </td>
            </tr>
            <tr>
                <td>11:45-12:15</td>
                <td>
                    <div>Morning break with refreshments</div>
                </td>
            </tr>
            <tr>
                <td>12:15-13:15</td>
                <td>
                    <div>Panel: Perspectives on Practical Reproducibility in Climate Science (<a href="../speakers/marion_weinzierl.html">Marion Weinzierl</a>, <a href="../speakers/dominic_orchard.html">Dominic Orchard</a>, <a href="../speakers/alejandro-coca-castro.html">Alejandro Coca-Castro</a>, Chair <a href="../team#mcs-and-session-chairs">Cassandra Gould van Praag</a>)</div>
                </td>
            </tr>
            <tr>
                <td>13:15-14:30</td>
                <td>
                    <div>Lunch</div>
                </td>
            </tr>
            <tr>
                <td>14:30-15:45</td>
                <td>
                    <div>Virtual <a href="https://www.eventsforce.net/turingevents/frontend/reg/tOtherPage.csp?pageID=150913&ef_sel_menu=2179&eventID=358">poster exhibition</a> and afternoon refreshments</div>
                </td>
            </tr>
            <tr>
                <td>15:45-16:45</td>
                <td>
                    <div>Lightning talks (Chair <a href="../team#mcs-and-session-chairs">Meghna Asthana</a>)</div>
                    <div>
                    <ol>
                    <li><a href="../speakers/kenza_tazi.html"> Precipitation prediction from large-scale climatic features over the Upper Indus Basin using Gaussian Processes (Kenza Tazi)</a></li>
                    <li><a href="../speakers/marc_girona-mata.html">Spatially-Coherent Probabilistic Downscaling of Daily Precipitation in Ungauged Mountain Locations: A Transfer Learning Study in the Swiss Alps and the Langtang Valley, Nepal (Marc Girona-Mata)</a></li>
                    <li><a href="../speakers/ilenia_manco.html">Machine Learning for Stochastic Parametrisation (Ilenia Manco)</a></li>
                    <li><a href="../speakers/peter_manshausen.html">Predicting visible ship tracks (Peter Manshausen)</a></li>
                    <li><a href="../speakers/daria_botvynko.html">Predicting visible ship tracks (Daria Botvynko)</a></li>
                    </ol>
                    </div>                
                </td>
            </tr>
            <tr>
                <td>16:50-17:50</td>
                <td>
                    <div><a href="../speakers/anima_anandkumar.html">Role of AI in tackling climate change (Anima Anandkumar)</a></div>
                </td>
            </tr>
            <tr>
                <td>17:50-18:00</td>
                <td>
                    <div>Closing remarks for Day 2 (<a href="../team#mcs-and-session-chairs">Orlando Timmerman</a> and <a href="../team#mcs-and-session-chairs">Andrew McDonald</a>)</div>
                </td>
            </tr>
            <tr>
                <td>18:30-onwards</td>
                <td>
                    <div>CI2024 Dinner at BMA House (in-person attendees only)</div>
                </td>
            </tr>
        </table>
    </div>
    <h5><a href="#anchor_top">Jump to top of schedule</a></h5>
</div>

<div id="schedule-04-24" class="schedule-block">
    <h4>Wednesday 24 April 2024</h4>

    <div class="schedule-content">
        <table class="osr-schedule">
            <tr>
                <td>UTC+1</td>
                <td>DAY 3</td>
            </tr>
            <tr>
                <td>09:00-09:30</td>
                <td>
                    <div>Registration with welcome refreshements</div>
                </td>
            </tr>
            <tr>
                <td>09:30-09:35</td>
                <td>
                    <div>Welcome back (<a href="../team#mcs-and-session-chairs">Cassandra Gould van Praag</a>)</div>
                </td>
            </tr>
            <tr>
                <td>09:35-10:40</td>
                <td>
                     <div>Lightning talks (Chair <a href="../team#mcs-and-session-chairs">Guillaume Couairon</a></div>
                    <div>
                    <ol>
                    <li><a href="../speakers/fiona_turner.html"> Building probabilistic projections of the Antarctic contribution to global sea level rise using a random forest emulator (Fiona Turner)</a></li>
                    <li><a href="../speakers/leo_edel.html">Reconstruction of Arctic sea ice thickness (1992-2010) based on a hybrid machine learning and data assimilation approach (Léo Edel)</a></li>
                    <li><a href="../speakers/ayush_prasad.html">Modeling Snow on Sea Ice using Physics Guided Machine Learning (Ayush Prasad)</a></li>
                    <li><a href="../speakers/harish_baki.html">Estimating high-resolution profiles of wind speeds from a global reanalysis dataset using TabNet (Harish Baki)</a></li>
                    <li><a href="../speakers/abhiraami_navaneethanathan.html">Estimating global ocean POC fluxes through machine learning and data fusion on heterogeneous and sparse in-situ observations (Abhiraami Navaneethanathan)</a></li>
                    <li><a href="../speakers/solomon_white.html">Improving ocean model generalisation by including water type classification as pre-processing to the satellite image (Solomon White)</a></li>
                    </ol>
                    </div> 
                </td>
            </tr>
            <tr>
                <td>10:40-11:10</td>
                <td>
                    <div>Morning break with refreshments</div>
                </td>
            </tr>
            <tr>
                <td>11:10-12:10</td>
                <td>
                    <div>Panel: Ethics and Explainability in Climate AI: From Theory to Practice (<a href="../speakers/elizabeth_barnes.html">Elizabeth Barnes </a>, <a href="../speakers/david-john_gagne.html">David-John Gagne</a>, <a href="../speakers/galen_mckinley.html">Galen McKinley</a>, <a href="../speakers/savannah_thais.html">Savannah Thais</a>, Chair <a href="../team#mcs-and-session-chairs">Viviana Acquaviva</a>)</div>
                </td>
            </tr>
            <tr>
                <td>12:10-13:10</td>
                <td>
                    <div>Lunch</div>
                </td>
            </tr>
            <tr>
                <td>13:10-14:15</td>
                <td>
                    <div>On Aerosol & Atmospheric Applications (Chair <a href="../team#mcs-and-session-chairs">Ricardo Barros Lourenço</a>)</div>
                    <div>
                    <ol>
                    <li><a href="../speakers/elena_fillola.html">Accelerating GHG emissions inference using Graph Neural Networks (Elena Fillola)</a></li>
                    <li><a href="../speakers/eliza_duncan.html">Untangling Aerosol Processes: Exploiting Explainable Machine Learning Techniques in a Lagrangian Framework (Eliza Duncan)</a></li>
                    <li><a href="../speakers/paolo_pelucchi.html">Towards probabilistic aerosol retrievals with invertible neural networks (Paolo Pelucchi)</a></li>
                    </ol>
                    </div>                
                </td>
            </tr>
            <tr>
                <td>14:20-15:20</td>
                <td>
                    <div><a href="../speakers/amy_mcgovern.html">How We are Building Trustworthy AI for Weather and Climate in AI2ES (Amy McGovern</a> and <a href="../speakers/david-john_gagne.html">David-John Gagne)</a></div>
                </td>
            </tr>
            <tr>
                <td>15:20-15:50</td>
                <td>
                    <div>Afternoon break with refreshments</div>
                </td>
            </tr>
            <tr>
                <td>15:50-16:05</td>
                <td>
                    <div>Closing remarks for Day 3 and conference close (<a href="../team#mcs-and-session-chairs">Cassandra Gould van Praag</a>)</div>
                </td>
            </tr> 
        </table>
    </div>
    <h5><a href="#anchor_top">Jump to top of schedule</a></h5>

</div>

<div class="schedule-leave-space-before-footer">
</div>


<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src='https://plugins.eventable.com/eventable.js';fjs.parentNode.insertBefore(js,fjs);}}(document,'script', 'eventable-script');</script>

