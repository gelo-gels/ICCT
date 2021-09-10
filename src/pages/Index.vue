<template>
  <q-page class="font-poppins container__index">
    <div class="row">

      <div class="col-md-4 col-sm-6 col-12">
        <div style="margin: 10px">
            <div class="ZoomBoxes">
              <div class="text-bold" style="font-size: 20px">
                HFIL11
                </div>
                <div style="font-size: 10px">
                  7:00 AM - 8:00 AM
                </div>
                <div style="font-size: 10px">
                  Fridays
                </div>

              <div style="font-size: 13px">
                <div class="q-mt-md">
                  Meeting ID: 95266896401 <i class="far fa-copy" />
                </div>
                <div>
                  Passcode: SHS1234 <i class="far fa-copy" />
                </div>
              </div>

              <div class="text-center">
                <div class="q-mt-md text-bold" style="font-size: 13px">
                  DATES
                </div>
                <div style="font-size: 12px">
                  <div> 
                    September 10, 17, 24
                  </div>
                  <div>
                    October 1, 8, 15, 29
                  </div>
                  <div>
                    November 12, 26
                  </div>  
                </div>
              </div>

              <div class="q-mt-md">
                <a style="text-decoration: none; color: #f0f9ff;" target="_blank" href="https://zoom.us/j/95266896401?pwd=WUdRYTZ1ZjRYcHE5OUZHN1dQU2Zvdz09">
                  <q-btn outline label="Zoom App" class="full-width" />
                </a>
              </div>
          </div>
        </div>
      </div>
      
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'PageIndex'
})
</script>


<style>
.ZoomBoxes {
  border: 1px solid #a1a1a1;
  padding: 20px;
  background-color: #002c4d;
  border-radius: 4px;
  width: 100%;
  height: 100%;
  cursor: pointer;
  transition: 1s;
}
.ZoomBoxes:hover {
  background-color: #003257;
}
.container__index {
  /* margin-left: 300px;
  margin-right: 300px; */
  max-width: 1000px;
  margin: 0 auto !important; 
	float: none !important; 
  padding: 30px 30px 0px 30px
}
</style>