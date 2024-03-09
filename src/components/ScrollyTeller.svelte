<h1 class = 'index'>index {index}</h1>


<Scroller
  top={0.0}
  bottom={1}
  threshold={0}

  bind:index
  bind:offset

>
  <div class="background" slot="background" >
    <div class="progress-bars">

      <!-- <p>till next page</p > -->
      <progress value={offset || 0} />

      <!-- <p>total progress</p >
      <progress value={progress || 0} /> -->
    </div>
  </div>

  <div class="foreground" slot="foreground" >

    {#if index === 0}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image1">
    <p class="topic">To Snitch or Not to Snitch: That is the Question<p>
      <p class="text1-1">You 🐱 committed a minor crime with your friend 🐶 and were sentenced to 1 year of prison . Now 👮🏻 suspect that you two committed a more serious crime other than this. You two have been arrested and put in separate rooms. </p >
      <br>
      <br>
      <p class="text1-2"> You can either <bold class = 'bolded'>stay silent (cooperate)</bold> or <bold class = 'bolded'>betray (defect).</bold> </p >
    {/if}
    
    {#if index === 1}
    <p class="text2"><bold class = 'bolded'>You can’t talk to each other</bold>, and you have no idea whether your friend stays silent or testifies against you.
    </p >
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image2">
    {/if}

    {#if index === 2}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image3">
    <p class="text3">If you choose to defect (betray) by admitting your friend committed the crime, and your friend chooses to cooperate (stay silent), you will go free. But your friend will be sentenced to 3 years of prison.</p >
    {/if}

    {#if index === 3}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image4">
    <p class="text4">But if you cooperate (stay silent), and your friend defects (betray) you, you’ll have to spend three years in prison and your friend goes free.</p >

    {/if}

    {#if index === 4}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image5">
    <p class="text5">If both of you choose to defect (betray), you will both have to stay in prison for 2 years.
    </p >
    {/if}

    {#if index === 5}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image6">
    <p class="text6">If both of you cooperate (stay silent), you both spend 1 year in prison only for the minor crime you are already arrested for.
    </p >
    {/if}

    {#if index === 6}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image7">
    <h2 class="text7">Let’s Summarize them into a Matrix Form:</h2 >
    {/if}

    {#if index === 7}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image8"> 
    <p class="text8">If both of you cooperate (stay silent), you both spend 1 year in prison.</p >
    {/if}

    {#if index === 8}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image9">
    <p class="text9">If one of you defects (betray), the betrayer goes free and the one who cooperates (stays silent) spends 3 years in prison.</p >
    {/if}

    {#if index === 9}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image10">
    <p class="text10">If both of you defect (betray), both of you spend 2 years in prison.</p >
    {/if}

    {#if index === 10}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image11">
    <svg id="slide-11" width="400" height="200" xmlns="http://www.w3.org/2000/svg">
      <rect class = "clicker" width="200" height="100"></rect>
    </svg>
    <p class="text11">What’s the best move if you think your friend is going to cooperate (stay silent)?
    </p >
    {/if}

    {#if index === 11}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image12">
    <p class="text12">(cooperate) If you choose to cooperate (stay silent), you will still stay in prison for 1 year. 

      Choosing to defect (betray) will free you instead. Therefore, the best move (assuming your friend will cooperate) is to defect them, so that you can be free.
      </p >

      <p class="text12">(cooperate) If you choose to cooperate (stay silent), you will still stay in prison for 1 year. 

        (defect) Since defecting (betray) will exempt you from going to jail, it’s reasonable why you choose to defect! Great Job!
        </p >
    {/if}

    {#if index === 12}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image13">
    <svg id="slide-13" width="400" height="200" xmlns="http://www.w3.org/2000/svg">
      <rect class = "clicker" width="200" height="100"></rect>
    </svg>
    <p class="text13">What’s the best move if you think your friend is going to defect?
    </p >
    {/if}

    {#if index === 13}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image14">
    <p class="text14">(cooperate) If you choose to cooperate (staying silent), you will still stay in prison for 3 years. 
      Choosing to defect (betray) will reduce it to 1 year  instead. Therefore, the best move (assuming your friend will defect) is to defect (betray) them. 
      </p >

      <p class="text14">(cooperate) If you choose to cooperate (staying silent), you will still stay in prison for 3 years. 
        (defect) Since defecting (betray) will reduce the sentence from 3 to 2 years, it’s reasonable why you choose to defect! Great Job!
        </p >
    {/if}

    <!-- {#if index === 14}
    <img src={slides[index]} alt={`Slide ${index + 1}`} class="slide-image15">
    {/if} -->

    <section> 1

    </section>
    <section> 2 

    </section>
    <section> 3  

    </section>
    <section> 4  

    </section>
    <section> 5 

    </section>
    <section> 6  

    </section>
    <section> 7 

    </section>
    <section> 8 

    </section>
    <section> 9  

    </section>
    <section> 10 
      <svg id = 'section10' class = "clicker" width="400" height="500" xmlns="http://www.w3.org/2000/svg">
      </svg>
    </section>
    <section> 11  

    </section>
    <section> 12  
      <svg id = "section12" class = "clicker" width="400" height="500" xmlns="http://www.w3.org/2000/svg">
      </svg>
    </section>
    <section> 13 

    </section>
    <section> 14 

    </section>
    <section> 15
    </section>
    </div>
</Scroller>

<script>
    import Scroller from "@sveltejs/svelte-scroller";
    import { select, selectAll } from 'd3-selection';
    let already_displayed10 = false;
    let already_displayed12 = false;


    let index, offset;
    import { onMount } from 'svelte';
    import * as d3 from 'd3';
  
    export let slides = [];
    var button10_1;
    var button10_2;

    var button12_1;
    var button12_2;


    $: {
      if (index === 10) {
        createClickers('#section10', 'blue');
        already_displayed10 = true;
        } else if (already_displayed10 === true) {
          button10_1.attr('display', 'none')
          button10_2.attr('display', 'none')        }

      if (index === 12) {
        createClickers('#section12', 'red');
        already_displayed12 = true;
        } else if (already_displayed12 === true) {
          button12_1.attr('display', 'none')
          button12_2.attr('display', 'none')
        }
      }


//      $: {
//       if (index === 10 | index === 12){
//         // button1.attr('display', 'inline')
//         // button2.attr('display', 'inline')
//         already_displayed = true
//       }
//       else if (already_displayed === true) {
//         button1.attr('display', 'none')
//         button2.attr('display', 'none')
//         // already_displayed = false;
//       }
// }

    //  $: {
    //   if (index === 10 | index === 12){
    //     already_displayed10 = true;
    //     already_displayed12 = true;

    //   }
    //   else if (already_displayed === true) {
    //     button1.attr('display', 'none')
    //     button2.attr('display', 'none')
    //     // already_displayed = false;
    //   }
    // }

    function createClickers(id, color) {

        const svg10_1 = d3.select('#section10');
        const svg10_2 = d3.select('#section10');

        const svg12_1 = d3.select('#section12');
        const svg12_2 = d3.select('#section12');

        if (id === '#section10') {
          button10_1 = svg10_1
              .append('rect')
              // .attr('display', 'none')
              .attr('x', 100) // X position
              .attr('y', 50)  // Y position
              .attr('width', 200) // Width
              .attr('height', 100) // Height
              .attr('fill', color) // Fill color
              .attr('stroke', 'light-purple') // Border color
              .attr('cursor', 'pointer') // Change cursor on hover
              .on('click', function(event) {
                console.log('clicked');
              })
              .on('mouseover', function(event, d) {
                console.log('mouseover');
              })
              .on('mouseout', function() {
                console.log('mouseout');
              });

          button10_2 = svg10_2
              .append('rect')
              // .attr('display', 'none')
              .attr('x', 100) // Adjust these attributes as necessary
              .attr('y', 200)
              .attr('width', 200)
              .attr('height', 100)
              .attr('fill', color) // Making it red for visibility
              .attr('stroke', 'black')
              .attr('cursor', 'pointer')
              .on('click', function() {
                console.log('clicked');
              });

        // Add a click event listener to the rectangle
        // button10_1.on('click', function() {
        //     alert('Rectangle button clicked!');
        // });

        // button10_2.on('click', function() {
        //     alert('Rectangle button clicked!');
        // });


      } 
      if (id === '#section12') {
          button12_1 = svg12_1
            .append('rect')
            // .attr('display', 'none')
            .attr('x', 100) // X position
            .attr('y', 50)  // Y position
            .attr('width', 200) // Width
            .attr('height', 100) // Height
            .attr('fill', color) // Fill color
            .attr('stroke', 'light-purple') // Border color
            .attr('cursor', 'pointer') // Change cursor on hover
            .on('click', function(event) {
              console.log('clicked');
              d3.event.stopPro
            })
            .on('mouseover', function(event, d) {
              console.log('mouseover');
            })
            .on('mouseout', function() {
              console.log('mouseout');
            });

          button12_2 = svg12_2
              .append('rect')
              // .attr('display', 'none')
              .attr('x', 100) // Adjust these attributes as necessary
              .attr('y', 200)
              .attr('width', 200)
              .attr('height', 100)
              .attr('fill', color) // Making it red for visibility
              .attr('stroke', 'black')
              .attr('cursor', 'pointer')
              .on('click', function() {
                console.log('clicked');
              });

        // Add a click event listener to the rectangle
        // button12_1.on('click', function() {
        //     alert('Rectangle button clicked!');
        // });

        // button12_2.on('click', function() {
        //     alert('Rectangle button clicked!');
        // });

      }
      

    }
  </script>
  
  
  <style>

   .index {
    position:fixed;
   }

   .topic{
      position:fixed;
      text-align: center;
      display:block;
      font-family: "Rye", serif;
      font-weight: 400;
      font-style: normal;
      font-size: 40px;
      max-height: 90vh;

      width: 100%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -600%);

    } 
    
    .text1-1 {
      position: fixed;
      text-align: center;
      max-height: 90vh;
      font-size: 30px;
      /* transform: translate(150px, 150px); */
      width: 80%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -180%);
    }

    .text1-2 {
      text-align: center;
      position: fixed;
      /* max-height: 90vh; */
      font-size: 30px;
      /* transform: translate(20px, 250px); */
      /* max-width: 80%; */
      width: 80%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -10%);
    }

    .text2 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -500%);
    }

    .text3 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -400%); /* changed from -200% to -400% */
    }

    .text4 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -400%); /* for double-line text */
    }

    .text5 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -800%); /* for single-line text*/
    }

    .text6 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -400%);
    }

    .text7 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 45px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -630%); /* for 'let's summarize...' */
    }

    .text8 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -900%); /* for single-line text*/
    }

    .text9 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -450%);
    }

    .text10 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -900%);
    }

    .text11 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -900%);
    }

    .text12 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -500%);
    }

    .text13 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -500%);
    }

    .text14 {
      position: fixed;
      text-align: center;
      /* max-height: 90vh; */
      font-size: 30px;
      width: 90%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -500%);
    }

    .slide-image1 {
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -15%) scale(40%);
      max-width: 90%;
      max-height: 90vh;

    }

    .slide-image2 {
      position: fixed;
      width: 80%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -30%) scale(70%);
    }

    .slide-image3 {
      position: fixed;
      width: 80%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -30%) scale(70%);
    }

    .slide-image4 {
      position: fixed;
      width: 80%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -30%) scale(70%);
    }

    .slide-image5 {
      position: fixed;
      width: 80%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -30%) scale(70%);
    }

    .slide-image6 {
      position: fixed;
      width: 80%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -30%) scale(70%);
    }

    .slide-image7 {
      position: fixed;
      width: 100%; /* changed from 80% t0 95% to make the matrix bigger */
      top: 40%; /* shift up by changing 50% to 40% */
      left: 50%;
      transform: translate(-50%, -40%) scale(40%);
    }

    .slide-image8 {
      position: fixed;
      width: 100%; /* changed from 80% t0 95% to make the matrix bigger */
      top: 40%; /* shift up by changing 50% to 40% */
      left: 50%;
      transform: translate(-50%, -40%) scale(40%);
    }

    .slide-image9 {
      position: fixed;
      width: 100%; /* changed from 80% t0 95% to make the matrix bigger */
      top: 40%;
      left: 50%;
      transform: translate(-50%, -40%) scale(40%);
    }

    .slide-image10 {
      position: fixed;
      width: 100%; /* changed from 80% t0 95% to make the matrix bigger */
      top: 40%; /* shift up by changing 50% to 40% */
      left: 50%;
      transform: translate(-50%, -40%) scale(40%);
    }
    .slide-image11 {
      position: fixed;
      width: 100%; /* changed from 80% t0 95% to make the matrix bigger */
      top: 40%; /* shift up by changing 50% to 40% */
      left: 50%;
      transform: translate(-50%, -40%) scale(40%);
    }

    .slide-image12 {
      position: fixed;
      width: 80%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -30%) scale(70%);
    }

    .slide-image13 {
      position: fixed;
      width: 100%; /* changed from 80% t0 95% to make the matrix bigger */
      top: 40%; /* shift up by changing 50% to 40% */
      left: 50%;
      transform: translate(-50%, -40%) scale(40%);
    }

    .slide-image14 {
      position: fixed;
      width: 80%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -40%) scale(40%);
    }

 [slot="background"] {
    position: fixed;
  background-color: rgba(0, 0, 0, 0);
  border-top: 2px solid #ff400000;
  border-bottom: 2px solid #ff400000;
  font-size: 1.4em;
  overflow: hidden;
  padding: 1em;
    transform: scale(0.7) translate(-20%, -30%);
 }
 
 [slot="foreground"] {
  pointer-events: none;
    text-align: center;
 }
/*  
 [slot="foreground"] section {
  pointer-events: all;
 } */
 
 section {
  height: 80vh;
  background-color: rgba(0, 0, 0, 0);
  color: rgb(7, 0, 0);
  padding: 1em;
  /* margin: 0 0 2em 0; */
 }


  .bolded {
    font-weight: bold;
  }

  .clicker {
    position: fixed;
    top:50%;
    left:50%;
    transform: translate(-50%, -50%);
    z-index: 1;
    /* display: block */
 }

  
  </style>