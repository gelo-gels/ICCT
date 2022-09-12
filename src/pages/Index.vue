<template>
  <q-page class="font-poppins">
    <div class="container__index">

    <div class="text-bold q-mb-md text-center dateToday" style="font-size: 24px">
        {{currentDateTime()}} 
    </div>

    <div class="text-center q-mb-md"> 
      <q-btn @click="$router.push({name: 'gallery'})" outline label="Gallery" class="q-px-xl" />
    </div>




    <div class="row">


      <!-- MONDAYS -->
      <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div :class="mon_6amTo7am.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes' &&
                         mon_7amTo8am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_8amTo9am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_9amTo10am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes'">
              <div class="text-bold" style="font-size: 20px">
                {{ mon_6amTo7am.section }}
                </div>
                <div style="font-size: 15px">
                 {{ mon_6amTo7am.time }}
                </div>
                <div style="font-size: 15px">
                  Mondays
                </div>

              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="mon_6amTo7am.meeting_link">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>

              </div>
          </div>
        </div>
      </div>






       <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div :class="mon_7amTo8am.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes' &&
                         mon_6amTo7am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_8amTo9am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_9amTo10am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes'">
              <div class="text-bold" style="font-size: 20px">
                {{ mon_7amTo8am.section }}
                </div>
                <div style="font-size: 15px">
                  {{ mon_7amTo8am.time }}
                </div>
                <div style="font-size: 15px">
                  Mondays
                </div>


              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="mon_7amTo8am.meeting_link">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>

              </div>
          </div>
        </div>
      </div>






      
      <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div :class="mon_10amTo11am.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes' &&
                         mon_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_6amTo7am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_7amTo8am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_8amTo9am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_9amTo10am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes'">
              <div class="text-bold" style="font-size: 20px">
                {{ mon_10amTo11am.section }}
                </div>
                <div style="font-size: 15px">
                  {{ mon_10amTo11am.time }}
                </div>
                <div style="font-size: 15px">
                  Mondays
                </div>

              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="mon_10amTo11am.meeting_link">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>

              </div>
          </div>
        </div>
      </div>



      <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div :class="mon_10amTo11am.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes' &&
                         mon_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_6amTo7am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_7amTo8am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_8amTo9am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_9amTo10am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes'">
              <div class="text-bold" style="font-size: 20px">
                {{ mon_11amTo12pm.section }}
                </div>
                <div style="font-size: 15px">
                  {{ mon_11amTo12pm.time }}
                </div>
                <div style="font-size: 15px">
                  Mondays
                </div>

              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="mon_11amTo12pm.meeting_link">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>

              </div>
          </div>
        </div>
      </div>

    <!-- END MONDAYS -->


    <!-- FRIDAYS -->

         <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div :class="fri_8amTo9am.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes' && 
                         mon_6amTo7am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_7amTo8am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         mon_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_9amTo10am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                         fri_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes'">
              <div class="text-bold" style="font-size: 20px">
                {{ fri_8amTo9am.section }}
                </div>
                <div style="font-size: 15px">
                  {{ fri_8amTo9am.time }}
                </div>
                <div style="font-size: 15px">
                  Fridays
                </div>

              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="fri_8amTo9am.meeting_link">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>

              </div>
          </div>
        </div>
      </div>







      <div class="col-md-4 col-sm-6 col-12">
              <div style="margin: 10px">
                  <div :class="fri_9amTo10am.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes' &&
                               mon_6amTo7am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                               mon_7amTo8am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                               mon_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                               mon_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                               fri_8amTo9am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                               fri_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                               fri_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes'">
                    <div class="text-bold" style="font-size: 20px">
                      {{ fri_9amTo10am.section }}
                      </div>
                      <div style="font-size: 15px">
                        {{ fri_9amTo10am.time }}
                      </div>
                      <div style="font-size: 15px">
                        Fridays
                      </div>

                    <div class="q-mt-md">
                      <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="fri_9amTo10am.meeting_link">
                        <q-btn outline label="Zoom App" class="full-width" />
                      </a>

                    </div>
                </div>
              </div>
            </div>





         <div class="col-md-4 col-sm-6 col-12">
          <div style="margin: 10px">
              <div :class="fri_10amTo11am.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes' &&
                           mon_6amTo7am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           mon_7amTo8am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           mon_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           mon_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           fri_8amTo9am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           fri_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           fri_9amTo10am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes'">
                <div class="text-bold" style="font-size: 20px">
                  {{ fri_10amTo11am.section }}
                  </div>
                  <div style="font-size: 15px">
                    {{ fri_10amTo11am.time }}
                  </div>
                  <div style="font-size: 15px">
                    Fridays
                  </div>

                <div class="q-mt-md">
                  <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="fri_10amTo11am.meeting_link">
                    <q-btn outline label="Zoom App" class="full-width" />
                  </a>

                </div>
            </div>
          </div>
        </div>


        <div class="col-md-4 col-sm-6 col-12">
          <div style="margin: 10px">
              <div :class="fri_10amTo11am.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes' &&
                           mon_6amTo7am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           mon_7amTo8am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           mon_10amTo11am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           mon_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           fri_8amTo9am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           fri_11amTo12pm.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes' &&
                           fri_9amTo10am.active == true ? 'ZoomInactiveBoxes' : 'ZoomBoxes'">
                <div class="text-bold" style="font-size: 20px">
                  {{ fri_11amTo12pm.section }}
                  </div>
                  <div style="font-size: 15px">
                    {{ fri_11amTo12pm.time }}
                  </div>
                  <div style="font-size: 15px">
                    Fridays
                  </div>

                <div class="q-mt-md">
                  <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="fri_11amTo12pm.meeting_link">
                    <q-btn outline label="Zoom App" class="full-width" />
                  </a>

                </div>
            </div>
          </div>
        </div>

    </div>

    </div>
  </q-page>
</template>

<script>
import { defineComponent, ref } from 'vue';
import moment from 'moment'

    export default defineComponent({
      name: 'PageIndex',

      data: () => 
        ({
          mon_6amTo7am: 
            { 
              section: 'OLHPHIL21',
              time: '6:00 AM - 7:00 AM', 
              meeting_link: 'https://us04web.zoom.us/j/5128036461?pwd=47izzaAuAirUWfLPbWYMmFfa5XcJOA.1',
              active: false
            },

          mon_7amTo8am: 
            { 
              section: 'HRES13',
              time: '7:00 AM - 8:00 AM', 
              meeting_link: 'https://icct-edu-ph.zoom.us/j/8378458803?pwd=YzZlYWRiSGhRVWtUQjZpWWR2Q0xWdz09',
              active: false
            },
            
          mon_10amTo11am: 
            { 
              section: 'HEMT',
              time: '10:00 AM - 11:00 AM', 
              meeting_link: 'https://zoom.us/j/8204643619?pwd=Umh5KzJ6L1AxbjRNWmtYZHI1dFMxQT09',
              active: false
            },

          mon_11amTo12pm: 
            { 
              section: 'HELS21',
              time: '11:00 AM - 12:00 PM', 
              meeting_link: 'https://us04web.zoom.us/j/2247871067?pwd=bS9KaTBsV2hkZGNrbmR3WGI5cWVnQT09',
              active: false
            },


          fri_8amTo9am: 
            { 
              section: 'HPHYE21',
              time: '8:00 AM - 9:00 AM', 
              meeting_link: 'https://us04web.zoom.us/j/4814601266?pwd=kaTwzmI8xam6MOTfuqdZOevIivgUQY.1',
              active: false
            },

          fri_9amTo10am: 
            { 
              section: 'HENTRE21',
              time: '9:00 AM - 10:00 AM', 
              meeting_link: 'https://us04web.zoom.us/j/6944441229?pwd=kLPvMzYXjPH6GExM8Ft1qcILoYhBxm.1',
              active: false
            },

          fri_10amTo11am: 
            { 
              section: 'HEMT',
              time: '10:00 AM - 11:00 AM', 
              meeting_link: 'https://zoom.us/j/8204643619?pwd=Umh5KzJ6L1AxbjRNWmtYZHI1dFMxQT09',
              active: false
            },

          fri_11amTo12pm: 
            { 
              section: 'HELS21',
              time: '10:00 AM - 11:00 AM', 
              meeting_link: 'https://us04web.zoom.us/j/2247871067?pwd=bS9KaTBsV2hkZGNrbmR3WGI5cWVnQT09',
              active: false
            },


            persistent: ref(false),
            timestamp: "",
            hideTest: true,
        }),

      created() 
        {
            setInterval(this.getNow, 1000);
        },

      methods: 
        {
            currentDateTime() 
            {
              return moment().format('MMMM DD, YYYY')
            },

             getNow: function() 
              {
                // return moment().format('h:mm A');
                const time = moment().format('ddd h a');
                this.timestamp = time;
                console.log(this.timestamp);


                if(this.timestamp == "Mon 6 am")
                {
                  this.mon_6amTo7am.active = true
                }
                else
                {
                  this.mon_6amTo7am.active = false
                }

                

                if(this.timestamp == "Mon 7 am")
                {
                  this.mon_7amTo8am.active = true
                }
                else
                {
                  this.mon_7amTo8am.active = false
                }


                
                if(this.timestamp == "Mon 10 am")
                {
                  this.mon_10amTo11am.active = true
                }
                else
                {
                  this.mon_10amTo11am.active = false
                }


                if(this.timestamp == "Mon 11 am")
                {
                  this.mon_11amTo12pm.active = true
                }
                else
                {
                  this.mon_11amTo12pm.active = false
                }


                
                if(this.timestamp == "Fri 8 am")
                {
                  this.fri_8amTo9am.active = true
                }
                else
                {
                  this.fri_8amTo9am.active = false
                }



                if(this.timestamp == "Fri 9 am")
                {
                  this.fri_9amTo10am.active = true
                }
                else
                {
                  this.fri_9amTo10am.active = false
                }



                if(this.timestamp == "Fri 10 am")
                {
                  this.fri_10amTo11am.active = true
                }
                else
                {
                  this.fri_10amTo11am.active = false 
                }


                if(this.timestamp == "Fri 11 am")
                {
                  this.fri_11amTo12pm.active = true
                }
                else
                {
                  this.fri_11amTo12pm.active = false 
                }

              },
        },
      })

    
</script>



<style>
.ZoomBoxes {
  padding: 20px;
  border-radius: 13px;
  width: 100%;
  height: 100%;
  cursor: pointer;
  transition: 1s;
  background: rgba( 0, 50, 87, 0.1);
  box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
  backdrop-filter: blur( 8.5px );
  -webkit-backdrop-filter: blur( 8.5px );
  border-radius: 10px;
  border: 1px solid rgba( 255, 255, 255, 0.18 );
}
.ZoomBoxes:hover {
  background-color: rgba( 0, 50, 87, 0.5);
  transform: scale(1.1);
  box-shadow: 0px 0px 100px 1px #e0e0e0;
}
.ZoomInactiveBoxes {
  padding: 20px;
  border-radius: 13px;
  width: 100%;
  height: 100%;
  cursor: pointer;
  transition: 1s;
  background: rgba( 0, 50, 87, 0.1);
  box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
  backdrop-filter: blur( 8.5px );
  -webkit-backdrop-filter: blur( 8.5px );
  border-radius: 10px;
  border: 1px solid rgba( 255, 255, 255, 0.18 );
}
.zoomActiveBoxes {
  padding: 20px;
  border-radius: 13px;
  width: 100%;
  height: 100%;
  cursor: pointer;
  transition: 1s;
  background-color: rgba( 0, 50, 87, 0.5);
  transform: scale(1.1);
  box-shadow: 0px 0px 100px 1px #e0e0e0;
  backdrop-filter: blur( 8.5px );
  -webkit-backdrop-filter: blur( 8.5px );
  border-radius: 10px;
  border: 1px solid rgba( 255, 255, 255, 0.18 );
}
.container__index {
  /* margin-left: 300px;
  margin-right: 300px; */
  max-width: 1000px;
  margin: 0 auto !important; 
	float: none !important; 
  padding: 30px 30px 0px 30px;
}
.dateToday {
  padding: 15px 10px;
  margin-left: 10px;
  margin-right: 10px;
  border-radius: 13px;
    background: rgba( 0, 50, 87, 0.1);
  box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
  backdrop-filter: blur( 8.5px );
  -webkit-backdrop-filter: blur( 8.5px );
  border-radius: 10px;
  border: 1px solid rgba( 255, 255, 255, 0.18 );
}
</style>

