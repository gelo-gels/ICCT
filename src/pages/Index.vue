<template>
  <q-page class="font-poppins container__index">


    <div class="text-bold q-mb-md text-center dateToday" style="font-size: 24px">
        {{currentDateTime()}}
    </div>



    <div class="row">


      <!-- MONDAYS -->
      <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div class="ZoomBoxes">
              <div class="text-bold" style="font-size: 20px">
                {{ mon_7amTo8am.section }}
                </div>
                <div style="font-size: 10px">
                 {{ mon_7amTo8am.time }}
                </div>
                <div style="font-size: 10px">
                  Mondays
                </div>

              <div style="font-size: 13px">
                <div class="q-mt-md">
                  Meeting ID: {{ mon_7amTo8am.meeting_id }}  <i class="far fa-copy" />
                </div>
                <div>
                  Passcode: {{ mon_7amTo8am.meeting_passcode }} <i class="far fa-copy" />
                </div>
              </div>

              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="mon_7amTo8am.meeting_link">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>

                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="mon_7amTo8am.edmodo_link">
                  <q-btn outline label="Edmodo" class="full-width q-mt-sm" />
                </a>
              </div>
          </div>
        </div>
      </div>






       <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div class="ZoomBoxes">
              <div class="text-bold" style="font-size: 20px">
                {{ mon_8amTo9am.section }}
                </div>
                <div style="font-size: 10px">
                  {{ mon_8amTo9am.time }}
                </div>
                <div style="font-size: 10px">
                  Mondays
                </div>

              <div style="font-size: 13px">
                <div class="q-mt-md">
                  Meeting ID: {{ mon_8amTo9am.meeting_id }} <i class="far fa-copy" />
                </div>
                <div>
                  Passcode: {{ mon_8amTo9am.meeting_passcode }} <i class="far fa-copy" />
                </div>
              </div>


              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="mon_8amTo9am.meeting_link">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>

                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="mon_8amTo9am.edmodo_link">
                  <q-btn outline label="Edmodo" class="full-width q-mt-sm" />
                </a>
              </div>
          </div>
        </div>
      </div>






      
      <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div class="ZoomBoxes">
              <div class="text-bold" style="font-size: 20px">
                {{ mon_9amTo10am.section }}
                </div>
                <div style="font-size: 10px">
                  {{ mon_9amTo10am.time }}
                </div>
                <div style="font-size: 10px">
                  Mondays
                </div>

              <div style="font-size: 13px">
                <div class="q-mt-md">
                  Meeting ID: {{ mon_9amTo10am.meeting_id }} <i class="far fa-copy" />
                </div>
                <div>
                  Passcode: {{ mon_9amTo10am.meeting_passcode }} <i class="far fa-copy" />
                </div>
              </div>

              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="mon_9amTo10am.meeting_link">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>

                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="mon_9amTo10am.edmodo_link">
                  <q-btn outline label="Edmodo" class="full-width q-mt-sm" />
                </a>
              </div>
          </div>
        </div>
      </div>

    <!-- END MONDAYS -->


    <!-- FRIDAYS -->

         <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div class="ZoomBoxes">
              <div class="text-bold" style="font-size: 20px">
                {{ fri_7amTo8am.section }}
                </div>
                <div style="font-size: 10px">
                  {{ fri_7amTo8am.time }}
                </div>
                <div style="font-size: 10px">
                  Fridays
                </div>

              <div style="font-size: 13px">
                <div class="q-mt-md">
                  Meeting ID: {{ fri_7amTo8am.meeting_id }} <i class="far fa-copy" />
                </div>
                <div>
                  Passcode: {{ fri_7amTo8am.meeting_passcode }} <i class="far fa-copy" />
                </div>
              </div>

              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="fri_7amTo8am.meeting_link">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>

                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="fri_7amTo8am.edmodo_link">
                  <q-btn outline label="Edmodo" class="full-width q-mt-sm" />
                </a>
              </div>
          </div>
        </div>
      </div>







      <div class="col-md-4 col-sm-6 col-12">
              <div style="margin: 10px">
                  <div class="ZoomBoxes">
                    <div class="text-bold" style="font-size: 20px">
                      {{ fri_8amTo9am.section }}
                      </div>
                      <div style="font-size: 10px">
                        {{ fri_8amTo9am.time }}
                      </div>
                      <div style="font-size: 10px">
                        Fridays
                      </div>

                    <div style="font-size: 13px">
                      <div class="q-mt-md">
                        Meeting ID: {{ fri_8amTo9am.meeting_id }} <i class="far fa-copy" />
                      </div>
                      <div>
                        Passcode: {{ fri_8amTo9am.meeting_passcode }} <i class="far fa-copy" />
                      </div>
                    </div>

                    <div class="q-mt-md">
                      <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="fri_8amTo9am.meeting_link">
                        <q-btn outline label="Zoom App" class="full-width" />
                      </a>

                      <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="fri_8amTo9am.edmodo_link">
                        <q-btn outline label="Edmodo" class="full-width q-mt-sm" />
                      </a>
                    </div>
                </div>
              </div>
            </div>





         <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div class="ZoomBoxes">
              <div class="text-bold" style="font-size: 20px">
                {{ fri_9amTo10am.section }}
                </div>
                <div style="font-size: 10px">
                  {{ fri_9amTo10am.time }}
                </div>
                <div style="font-size: 10px">
                  Fridays
                </div>

              <div style="font-size: 13px">
                <div class="q-mt-md">
                  Meeting ID: {{ fri_9amTo10am.meeting_id }} <i class="far fa-copy" />
                </div>
                <div>
                  Passcode: {{ fri_9amTo10am.meeting_passcode }} <i class="far fa-copy" />
                </div>
              </div>

              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="fri_9amTo10am.meeting_link">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>

                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" :href="fri_9amTo10am.edmodo_link">
                  <q-btn outline label="Edmodo" class="full-width q-mt-sm" />
                </a>
              </div>
          </div>
        </div>
      </div>







    </div>


  <div class="text-center">
    <q-btn class="text-bold q-mb-md text-center dateToday q-mt-xl" style="font-size: 24px; cursor: pointer"  @click="persistent = true">
        PSST POGI PAPINDOT AKO
    </q-btn>
  </div>
    
    <q-dialog v-model="persistent" persistent maximized>
      <q-card class="bg-transparent text-white">
        
        <q-img src="https://i.imgur.com/5wYBMwc.png" style="width: 100%; height: 100%">
        
          

          <div class="absolute-top-left bg-transparent text-subtitle1 text-center">
            <q-btn flat v-close-popup>
            gago
          </q-btn>
          </div>
        </q-img>

      </q-card>
    </q-dialog>

  </q-page>
</template>

<script>
import { defineComponent, ref } from 'vue';
import moment from 'moment'

    export default defineComponent({
      name: 'PageIndex',

      data: () => 
        ({
          mon_7amTo8am: 
            { 
              section: 'OLHPFP12',
              time: '7:00 AM - 8:00 AM', 
              meeting_id: '', 
              meeting_passcode: '',
              meeting_link: '',
              edmodo_link: ''
            },

          mon_8amTo9am: 
            { 
              section: 'OLHSOSC12',
              time: '8:00 AM - 9:00 AM', 
              meeting_id: '', 
              meeting_passcode: '',
              meeting_link: '',
              edmodo_link: ''
            },
            
          mon_9amTo10am: 
            { 
              section: 'OLHPHYE12',
              time: '9:00 AM - 10:00 AM', 
              meeting_id: '', 
              meeting_passcode: '',
              meeting_link: '',
              edmodo_link: ''
            },


          fri_7amTo8am: 
            { 
              section: 'OLHENG12',
              time: '7:00 AM - 8:00 AM', 
              meeting_id: '9858347560', 
              meeting_passcode: 'SHS2022',
              meeting_link: 'https://zoom.us/j/9858347560',
              edmodo_link: ''
            },

          fri_8amTo9am: 
            { 
              section: 'OLHFIL12',
              time: '8:00 AM - 9:00 AM', 
              meeting_id: '', 
              meeting_passcode: '',
              meeting_link: '',
              edmodo_link: ''
            },

          fri_9amTo10am: 
            { 
              section: 'OLHMATH12',
              time: '9:00 AM - 10:00 AM', 
              meeting_id: '', 
              meeting_passcode: '',
              meeting_link: '',
              edmodo_link: ''
            },


            persistent: ref(false)
        }),

      methods: {
      currentDateTime() {
        return moment().format('MMMM DD YYYY')
      }
  },

      mounted() {

        if( this.mon_7amTo8am.meeting_id == '')
        {
          this.mon_7amTo8am.meeting_id = 'Unavailable'
        }
        if( this.mon_7amTo8am.meeting_passcode == '')
        {
          this.mon_7amTo8am.meeting_passcode = 'Unavailable'
        }


        if( this.mon_8amTo9am.meeting_id == '')
        {
          this.mon_8amTo9am.meeting_id = 'Unavailable'
        }
        if( this.mon_8amTo9am.meeting_passcode == '')
        {
          this.mon_8amTo9am.meeting_passcode = 'Unavailable'
        }


        if( this.mon_9amTo10am.meeting_id == '')
        {
          this.mon_9amTo10am.meeting_id = 'Unavailable'
        }
        if( this.mon_9amTo10am.meeting_passcode == '')
        {
          this.mon_9amTo10am.meeting_passcode = 'Unavailable'
        }


        if( this.fri_7amTo8am.meeting_id == '')
        {
          this.fri_7amTo8am.meeting_id = 'Unavailable'
        }
        if( this.fri_7amTo8am.meeting_passcode == '')
        {
          this.fri_7amTo8am.meeting_passcode = 'Unavailable'
        }


        if( this.fri_8amTo9am.meeting_id == '')
        {
          this.fri_8amTo9am.meeting_id = 'Unavailable'
        }
        if( this.fri_8amTo9am.meeting_passcode == '')
        {
          this.fri_8amTo9am.meeting_passcode = 'Unavailable'
        }


        if( this.fri_9amTo10am.meeting_id == '')
        {
          this.fri_9amTo10am.meeting_id = 'Unavailable'
        }
        if( this.fri_9amTo10am.meeting_passcode == '')
        {
          this.fri_9amTo10am.meeting_passcode = 'Unavailable'
        }
      }
    });


    
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