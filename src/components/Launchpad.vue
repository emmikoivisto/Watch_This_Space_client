<template lang="html">
    <section>
        <!-- <h2>Hedgehog adventure time</h2> -->
        <div class="circular-sb">
            <p v-if="countdown>0">Welcome <br> Astronaut! <br> 
            Help our rocket to launch - answer enough questions correctly to get us home ! 
            <br> Pick a planet to <br> start the quiz...</p>
            <p v-if="countdown<=0">Thanks for your help - lets go explore some more!<p>
            <div class="circle1"></div>
            <div class="circle2"></div>
        </div>
        <!-- <img src="" alt=""> -->
    </section>
</template>

<script>
export default {
    name: 'launchpad',
    props: ['countdown']
    
}
</script>

<style lang="css" scoped>

section{
    background-image: url(../assets/hedgehogs-astronauts-sitting-planet_77984-964.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-color: #243141;
    height: 48vh;
    margin: 0px;
    color: #243141;
    padding: 40px;
}

h2 {
  color: #ff6a66;
  font-size: 2em;
  margin-top: 0px;
  margin-bottom: 0px;
  padding-top: 40px;
  padding-left: 90px;
  text-shadow: 2px 2px 6px #243141;
}

p {
  letter-spacing: 3pt;
  line-height: 20pt;
  /* font-family: Arial, Helvetica, sans-serif; */
}

.circular-sb {
  width: 350px;
  border: 5px solid #ff6a66;
  padding: 20px 0px;
  /* margin: 0px auto; */
  border-radius: 50%;
  text-align: center;
  /* font-size: 24px;
  font-weight: 900; */
  /* font-family: arial; */
  position: relative;
  color: #243141;
  background-color: rgba( 255, 255, 255, 0.8);
}

.circle1 {
  border: 5px solid #ff6a66;
  position: absolute;
  width: 25px;
  padding: 20px;
  border-radius: 50%;
  right: -15px;
  bottom: 190px;
  background-color: rgba( 255, 255, 255, 0.8);
}

.circle2 {
  border: 5px solid #ff6a66;
  position: absolute;
  width: 5px;
  padding: 10px 15px;
  border-radius: 50%;
  right: -60px;
  bottom: 170px;
  background-color: rgba( 255, 255, 255, 0.8);
}

</style>