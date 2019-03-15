<template>
<section>
    <h2>Education</h2>
    <TimeLine v-for="timeItem in timeline_data"
      v-bind:year="timeItem.year"
      v-bind:list="timeItem.list"
    />
</section>

</template>
<script>
import TimeLine from './timeline-vuejs/timeline-vuejs'


export default {
  components: {
    TimeLine,
  },
  data() {
     return {
       timeline_data: [
         {
           year: 2008,
           list:
           [
             {
               day: 15,
               month: "Dec",
               companyName: "University of León (Spain)",
              companyDescription: "Industrial Engineering, specializing in electricity and electronics. Level 6 MECU",
               web: "https://www.unileon.es/",
               text:`
               <p>Ability to work as an electronic, mechatronic, electrical and facillity engineer.</p>`
             }
           ]
         },
         {
           year: 2008,
           list:
           [
             {
               day: 22,
               month: "Jun",
               companyName: "University of Passo Fundo (Brazil)",
              companyDescription: "Foreign Exchange of annual duration",
               web: "https://www.upf.br/",
               text:`               <p>Ability to work as an electronic, mechatronic, electrical and facillity engineer.</p>
               <p> Portuguese Course </p> `
             }
           ]
         },
         {
           year: 2005,
           list:
           [
             {
               day: 28,
               month: "Apr",
               companyName: "Businessman Association of Leon",
              companyDescription: "Entrepreneurship and Selfemployment",
               web: "https://fele.es/",
               text:`Accounting, payroll, marketing and tax law. (300 hours) `
             }
           ]
         },
         {
           year: 2004,
           list:
           [
             {
               day: 20,
               month: "Oct",
               companyName: "University of León",
              companyDescription: "Programmable automation control system",
               web: "https://www.unileon.es/",
               text:`<p>Programming and commissioning of Programmable Logic Controllers (PLC) and SCADA .</p> `
             }
           ]
         },
         {
           year: 1999,
           list:
           [
             {
               day: 14,
               month: "Sept",
               companyName: "Don Bosco Institute",
              companyDescription: "C.O.U. ",
               web: "http://cdbosco.com/",
               text:`<p>Secondary education.</p> `
             }
           ]
         }
       ]
     }
   }
 }



</script>
