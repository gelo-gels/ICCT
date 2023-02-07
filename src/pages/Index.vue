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
      <div class="col-sm-4 col-md-2 col-12">
          <div style="margin: 10px">
            <div :class="monday.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes'">
              <div class="text-bold text-center" style="font-size: 20px">
                Monday
              </div>
            </div>
          </div>
          <div style="margin: 10px">
            <div :class="monday.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes'">
              <div class="text-center text-bold" style="font-size: 15px; color: red">
                FACE TO FACE
              </div>

              <div>

              <a href="https://us05web.zoom.us/j/9642197356?pwd=TEw3b05Iang4T1BCWUtXdUZhUVlSZz09" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px" >
                  <div style="text-decoration: underline;">
                    TVPROG3
                  </div>
                  <div>
                    8:00 - 9:00AM
                  </div>
                  <div>
                    Mr. Jasper
                  </div>
                </div>
              </a>

              <a href="https://us04web.zoom.us/j/3156411146?pwd=g96fTmNLtShDaaAvADPu6Reh1U1HgY.1" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px">
                  <div style="text-decoration: underline;">
                    OLHMI
                  </div>
                  <div>
                    11:00 - 12:00NN
                  </div>
                  <div>
                    Mr. Danilo
                  </div>
                </div>
              </a>

              <a href="https://us05web.zoom.us/j/6066844141?pwd=UXVMQkNNWDR5am5MU3QzMEpMUm4wUT09" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px" >
                  <div style="text-decoration: underline;">
                    HPS22
                  </div>
                  <div>
                    2:00 - 3:00PM
                  </div>
                  <div>
                    Ms. Mercy
                  </div>
                </div>
              </a>

              <a target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px; visibility: hidden" >
                  <div style="text-decoration: underline;">
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                </div>
              </a>

              </div>
            </div>
          </div>
        </div>

        <div class="col-sm-4 col-md-2 col-12">
          <div style="margin: 10px">
            <div :class="tuesday.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes'">
              <div class="text-bold text-center" style="font-size: 20px">
                Tuesday
              </div>
            </div>
          </div>
          <div style="margin: 10px">
            <div :class="tuesday.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes'">
              <div class="text-center text-bold" style="font-size: 15px; color: red">
                ONLINE
              </div>

              <div>

              <a href="https://us05web.zoom.us/j/9642197356?pwd=TEw3b05Iang4T1BCWUtXdUZhUVlSZz09" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px" >
                  <div style="text-decoration: underline;">
                    TVPROG3
                  </div>
                  <div>
                    12:00 - 1:00PM
                  </div>
                  <div>
                    Mr. Jasper
                  </div>
                </div>
              </a>

              <a href="https://us04web.zoom.us/j/4949080796?pwd=R8D5UNyPO2fHE6BUJXaIfHgvRwl2XL.1" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px">
                  <div style="text-decoration: underline;">
                    HRES
                  </div>
                  <div>
                    4:00 - 5:00PM
                  </div>
                  <div>
                    (ST) Ms. Mariz
                  </div>
                </div>
              </a>

              <a target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px; visibility: hidden" >
                  <div style="text-decoration: underline;">
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                </div>
              </a>

              <a target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px; visibility: hidden" >
                  <div style="text-decoration: underline;">
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                </div>
              </a>

              </div>
            </div>
          </div>
        </div>

        <div class="col-sm-4 col-md-2 col-12">
          <div style="margin: 10px">
            <div :class="wednesday.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes'">
              <div class="text-bold text-center" style="font-size: 20px">
                Wednesday
              </div>
            </div>
          </div>
          <div style="margin: 10px">
            <div :class="wednesday.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes'">
              <div class="text-center text-bold" style="font-size: 15px; color: red">
                ONLINE
              </div>

              <div>

              <a href="https://icct-edu-ph.zoom.us/j/8378458803?pwd=YzZlYWRiSGhRVWtUQjZpWWR2Q0xWdz09" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px" >
                  <div style="text-decoration: underline;">
                    HCL21
                  </div>
                  <div>
                    3:00 - 4:00PM
                  </div>
                  <div>
                    (ST) Mr. Daniel
                  </div>
                </div>
              </a>

              <a href="https://us04web.zoom.us/j/4949080796?pwd=R8D5UNyPO2fHE6BUJXaIfHgvRwl2XL.1" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px">
                  <div style="text-decoration: underline;">
                    HRES
                  </div>
                  <div>
                    4:00 - 5:00PM
                  </div>
                  <div>
                    (ST) Ms. Mariz
                  </div>
                </div>
              </a>

              <a target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px; visibility: hidden" >
                  <div style="text-decoration: underline;">
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                </div>
              </a>

              <a target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px; visibility: hidden" >
                  <div style="text-decoration: underline;">
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                </div>
              </a>

              </div>
            </div>
          </div>
        </div>

        <div class="col-sm-4 col-md-2 col-12">
          <div style="margin: 10px">
            <div :class="thursday.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes'">
              <div class="text-bold text-center" style="font-size: 20px">
                Thursday
              </div>
            </div>
          </div>
          <div style="margin: 10px">
            <div :class="thursday.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes'">
              <div class="text-center text-bold" style="font-size: 15px; color: red">
                ONLINE
              </div>

              <div>

              <a href="https://us05web.zoom.us/j/6066844141?pwd=UXVMQkNNWDR5am5MU3QzMEpMUm4wUT09" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px" >
                  <div style="text-decoration: underline;">
                    HPS22
                  </div>
                  <div>
                    12:00 - 1:00PM
                  </div>
                  <div>
                    Ms. Mercy
                  </div>
                </div>
              </a>

              <a href="https://icct-edu-ph.zoom.us/j/8378458803?pwd=YzZlYWRiSGhRVWtUQjZpWWR2Q0xWdz09" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px">
                  <div style="text-decoration: underline;">
                    HCL21
                  </div>
                  <div>
                    3:00 - 4:00PM
                  </div>
                  <div>
                    (ST) Mr. Daniel
                  </div>
                </div>
              </a>

              <a target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px; visibility: hidden" >
                  <div style="text-decoration: underline;">
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                </div>
              </a>
              
              <a target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px; visibility: hidden" >
                  <div style="text-decoration: underline;">
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                </div>
              </a>

              </div>
            </div>
          </div>
        </div>

        <div class="col-sm-4 col-md-2 col-12">
          <div style="margin: 10px">
            <div :class="friday.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes'">
              <div class="text-bold text-center" style="font-size: 20px">
                Friday
              </div>
            </div>
          </div>
          <div style="margin: 10px">
            <div :class="friday.active == true ? 'zoomActiveBoxes' : 'ZoomBoxes'">
              <div class="text-center text-bold" style="font-size: 15px; color: red">
                ONLINE
              </div>

              <div>

              <a href="https://us05web.zoom.us/j/9642197356?pwd=TEw3b05Iang4T1BCWUtXdUZhUVlSZz09" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px" >
                  <div style="text-decoration: underline;">
                    TVPROG3
                  </div>
                  <div>
                    12:00 - 1:00PM
                  </div>
                  <div>
                    Mr. Jasper
                  </div>
                </div>
              </a>

              <a href="https://us04web.zoom.us/j/3156411146?pwd=g96fTmNLtShDaaAvADPu6Reh1U1HgY.1" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px">
                  <div style="text-decoration: underline;">
                    OLHMI
                  </div>
                  <div>
                    2:00 - 3:00PM
                  </div>
                  <div>
                    Mr. Danilo
                  </div>
                </div>
              </a>

              <a href="https://icct-edu-ph.zoom.us/j/8378458803?pwd=YzZlYWRiSGhRVWtUQjZpWWR2Q0xWdz09" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px" >
                  <div style="text-decoration: underline;">
                    HCL21
                  </div>
                  <div>
                    3:00 - 4PM
                  </div>
                  <div>
                    (ST) Mr. Daniel
                  </div>
                </div>
              </a>
              
              <a href="https://us04web.zoom.us/j/4949080796?pwd=R8D5UNyPO2fHE6BUJXaIfHgvRwl2XL.1" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px" >
                  <div style="text-decoration: underline;">
                    HRES
                  </div>
                  <div>
                    4:00 - 5:00PM
                  </div>
                  <div>
                    (ST) Ms. Mariz
                  </div>
                </div>
              </a>

              </div>
            </div>
          </div>
        </div>

        <div class="col-sm-4 col-md-2 col-12">
          <div style="margin: 10px">
            <div class="ZoomBoxes">
              <div class="text-bold text-center" style="font-size: 20px">
                Saturday
              </div>
            </div>
          </div>
          <div style="margin: 10px">
            <div class="ZoomBoxes">
              <div class="text-center text-bold" style="font-size: 15px; color: red">
                GALA DAY
              </div>

              <div>

              <a href="https://scontent.fmnl17-2.fna.fbcdn.net/v/t1.6435-9/40427411_598401350557863_4158715510143320064_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=174925&_nc_eui2=AeFmY4lhDmRQh0zeUREVmInjzl7_ZqA3r-XOXv9moDev5ZItwJZSJOFqjg9sM957jXEnmQ0Z54p62aygDdc-tcQl&_nc_ohc=Rsp8uuYYcc8AX9eohE-&_nc_ht=scontent.fmnl17-2.fna&oh=00_AfBi8VRzSqiHnxQC_CKVFatSJCKpkJTMb4lAuVYiSPjYcw&oe=64040E1B" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px;">
                  <div style="text-decoration: underline; visibility: hidden">
                    blank
                  </div>
                  <div>
                    Lucky Calibara
                  </div>
                  <div style="visibility: hidden">
                    blank
                  </div>
                </div>
              </a>

              <a href="https://scontent.fmnl17-1.fna.fbcdn.net/v/t1.15752-9/329011172_1620537118368549_5294982453361485063_n.png?_nc_cat=101&ccb=1-7&_nc_sid=ae9488&_nc_eui2=AeFknUYxpZXfnWVrPH1lzSCCRMGFhD7aoMZEwYWEPtqgxiddb5txjBDUZ_iIAl7pToxpC_rh9a3RkXTItqfbTdAl&_nc_ohc=08p_YyeYN-UAX_0bMee&_nc_ht=scontent.fmnl17-1.fna&oh=03_AdSpcTNk9nuSRRWMYcEBQ6vdqS2RCunEbvPDDB06263ajA&oe=640421EA" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px;" >
                  <div style="text-decoration: underline; visibility: hidden">
                    blank
                  </div>
                  <div>
                    Jopay
                  </div>
                  <div style="visibility: hidden">
                    blank
                  </div>
                </div>
              </a>

             <a href="https://scontent.fmnl17-1.fna.fbcdn.net/v/t1.15752-9/260816106_249713733811598_8801772581978057508_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=ae9488&_nc_eui2=AeGY_ZcMFYYOyBkScFR5yTE68YpsgpDlmxnximyCkOWbGeapUVF-0bnrPeIqT64mpki_h0y_T0GXZOmSwaOHwk3G&_nc_ohc=sULmVGDLeQMAX8seaA-&_nc_ht=scontent.fmnl17-1.fna&oh=03_AdTa6W71IPhXfXWsE3LxnbAN2pcYqP2BZrFdK91BpkeHZQ&oe=64040F9B" target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px;" >
                  <div style="text-decoration: underline; visibility: hidden">
                    blank
                  </div>
                  <div>
                    Asim
                  </div>
                  <div style="visibility: hidden">
                    blank
                  </div>
                </div>
              </a>
              
             <a target="_blank" style="text-decoration: none">
                <div class="text-center text-bold ZoomBoxes" style="font-size: 15px; color: white; margin-top: 15px; visibility: hidden" >
                  <div style="text-decoration: underline;">
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                  <div>
                    blank
                  </div>
                </div>
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
            persistent: ref(false),
            timestamp: "",
            hideTest: true,

            monday: { active: false },
            tuesday: { active: false },
            wednesday: { active: false },
            thursday: { active: false },
            friday: { active: false },
        }),

      created() 
        {
            setInterval(this.getNow, 1000);
        },

      methods: 
        {
            currentDateTime() 
            {
              return moment().format('MMMM DD, YYYY | dddd')
            },

             getNow: function() 
              {
                // return moment().format('h:mm A');
                const time = moment().format('ddd h a');
                this.timestamp = time;
                console.log(this.timestamp);


                if(this.timestamp == "Mon 8 am" || this.timestamp == "Mon 11 am" || this.timestamp == "Mon 2 pm")
                {
                  this.monday.active = true
                }
                else
                {
                  this.monday.active = false 
                }



                if(this.timestamp == "Tue 12 pm" || this.timestamp == "Tue 4 pm")
                {
                  this.tuesday.active = true
                }
                else
                {
                  this.tuesday.active = false 
                }


                if(this.timestamp == "Wed 3 pm" || this.timestamp == "Wed 4 pm")
                {
                  this.wednesday.active = true
                }
                else
                {
                  this.wednesday.active = false 
                }


                if(this.timestamp == "thu 12 pm" || this.timestamp == "thu 3 pm")
                {
                  this.thursday.active = true
                }
                else
                {
                  this.thursday.active = false 
                }



                if(this.timestamp == "Fri 12 pm" || this.timestamp == "Fri 2 pm" || this.timestamp == "Fri 3 pm" || this.timestamp == "Fri 4 pm")
                {
                  this.friday.active = true
                }
                else
                {
                  this.friday.active = false 
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
/*.ZoomBoxes:hover {
  background-color: rgba( 0, 50, 87, 0.5);
  transform: scale(1.1);
  box-shadow: 0px 0px 100px 1px #e0e0e0;
}*/
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
  box-shadow: 0px 0px 100px 1px #e0e0e0;
  backdrop-filter: blur( 8.5px );
  -webkit-backdrop-filter: blur( 8.5px );
  border-radius: 10px;
  border: 1px solid rgba( 255, 255, 255, 0.18 );
}
.container__index {
  /* margin-left: 300px;
  margin-right: 300px; */
  max-width: 1500px;
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

