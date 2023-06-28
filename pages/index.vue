<template>
  <div>
    <div v-for="(card,i) in cards" :key="i">
        <v-card @click="toDetail()">
          <v-row>
            <v-col cols="2">
              <v-img
                cover
                src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"
                width="100%"
              >
              </v-img
            ></v-col>
            <v-col cols="10">
              <v-row>
                <v-col cols="6">
                  {{ card.title }}
                </v-col>
                <v-col cols="2">
                  <v-chip>{{ card.status }}</v-chip>
                </v-col>
                <v-col cols="2">
                  <p>{{ card.kilomate }}</p>
                </v-col>
                <v-col cols="2">
                  <v-chip class="ma-2" color="" outlined>
                    <v-icon left> mdi-car </v-icon>
                    {{ card.time }}
                  </v-chip>
                </v-col>
              </v-row>
              {{ card.address }}
            </v-col>
          </v-row>
        </v-card>
      </div>
    </div>
</template>
<script>
  export default {
    data: () => ({ value: 'recent' ,
      cards:[
          {
            title:"สถานี Charge",
            status:"เปิด",
            kilomate:"0.3 km",
            time:"3 นาที",
            address:"อ.เมือง จ.ขอนแแก่น 40000"

          },
              {
            title:"สถานี Charge",
            status:"เปิด",
            kilomate:"0.3 km",
            time:"3 นาที",
            address:"อ.เมือง จ.ขอนแแก่น 40000"

          },
              {
            title:"สถานี Charge",
            status:"เปิด",
            kilomate:"0.3 km",
            time:"3 นาที",
            address:"อ.เมือง จ.ขอนแแก่น 40000"

          },
              {
            title:"สถานี Charge",
            status:"ปิด",
            kilomate:"0.3 km",
            time:"3 นาที",
            address:"อ.เมือง จ.ขอนแแก่น 40000"

          },
              {
            title:"สถานี Charge",
            status:"เปิด",
            kilomate:"0.3 km",
            time:"3 นาที",
            address:"อ.เมือง จ.ขอนแแก่น 40000"

          },
              {
            title:"สถานี Charge",
            status:"เปิด",
            kilomate:"0.3 km",
            time:"3 นาที",
            address:"อ.เมือง จ.ขอนแแก่น 40000"

          },
              {
            title:"สถานี Charge",
            status:"ปิด",
            kilomate:"0.3 km",
            time:"3 นาที",
            address:"อ.เมือง จ.ขอนแแก่น 40000"

          }
        ]
    }),
    methods :{
      toDetail(){

      }
    }
  }
</script>
  
