<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Flter v-bind:artists="artists"/>
    <Test v-bind:artists="artists"/>
  </div>
</template>

<script>
import Test from './components/Test.vue'
import Flter from './components/Flter.vue'
export default {
  name: 'app',
  components: {
    Flter,
    Test
  },
    data (){
    return {
      artists: [
       
    {"id": 1, "quote":"That's thirty minutes away. I'll be there in ten.","context":"Pulp Fiction","source":"The Wolf","theme":"movies"},

    {"id": 2, "quote":"The first rule of Fight Club is: you do not talk about Fight Club. The second rule of Fight Club is: you DO NOT talk about Fight Club.","context":"Fight Club","source":"Tyler Durden", "theme":"movies"},

    {"id": 3, "quote":"My momma always said, ‘Life was like a box of chocolates. You never know what you’re gonna get.", "context":"Forrest Gump", "source":"Forrest Gump", "theme":"movies"},

    {"id": 4, "quote":"Ray, next time someone asks you if you’re a god, you say YES!","context":"Ghostbusters","source":"Winston Zeddemore","theme":"movies"},

    {"id": 5, "quote":"They’ve done studies, you know. Sixty percent of the time, it works every time.","context":"Anchorman","source":"Brian Fantana","theme":"movies"},

    {"id": 6, "quote":"This is so bad it’s gone past good and back to bad again.","context":"Ghost World","source":"Enid","theme":"movies"},

    {"id": 7, "quote":"Go that way, really fast. If something gets in your way, turn.","context":"Better Off Dead","source":"Charles De Mar","theme":"movies"},

    {"id": 8, "quote":"Put. That coffee. Down. Coffee's for closers only.","context":"Glengarry Glen Ross","source":"Blake","theme":"movies"},

    {"id": 9, "quote":"Good? Bad? I'm the guy with the gun.","context":"Army of Darkness","source":"Ash","theme":"movies"},

    {"id": 10, "quote":"Are you gonna bark all day, little doggy, or are you gonna bite?","context":"Reservoir Dogs","source":"Mr. Blonde","theme":"movies"},

    {"id": 11, "quote":"There are two types of people in the world - those with a gun, and those who dig. Now dig!","context":"The Good, the Bad, and the Ugly","source":"Blondie","theme":"movies"},

    {"id": 12, "quote":"If you try to run, I've got six little friends and they can all run faster than you can.","context":"From Dusk Til Dawn","source":"Seth","theme":"movies"},

    {"id": 13, "quote":"Are you gonna do something? Or just stand there and bleed?","context":"Tombstone","source":"Wyatt Earp","theme":"movies"},

    {"id": 14, "quote":"I love the smell of napalm in the morning","context":"Apocalypse now","source":"Kilgore","theme":"movies"},

    {"id": 15, "quote":"I could be the walrus. I'd still have to bum rides off people","context":"Ferris Bueller's Day Off","source":"Ferris","theme":"movies"},

    {"id": 16, "quote":"You either die a hero, or live long enough to see yourself become the villain.","context":"The Dark Knight","source":"Harvey Dent","theme":"movies"},

    {"id": 17, "quote":"If you hold back anything, I'll kill ya. If you bend the truth or I think you're bending the truth, I'll kill ya. If you forget anything, I'll kill ya. In fact, you're gonna have to work very hard to stay alive, Nick. Now, do you understand everything I've just said? 'Cause if you don't, I'll kill ya! Now, Mr Bubble and Squeak, you may enlighten me.","context":"Lock, Stock and Two Smoking Barrels","source":"Rory Breaker","theme":"movies"},

    {"id": 18, "quote":"You should never underestimate the predictability of stupidity.","context":"Snatch","source":"Bullet Tooth Tony","theme":"movies"},

    {"id": 19, "quote":"In the quiet words of the Virgin Mary... come again? ","context":"Snatch","source":"Brick Top","theme":"movies"},

    {"id": 20, "quote":"Heavy is good, heavy is reliable. If it doesn't work you can always hit them with it. ","context":"Snatch","source":"Boris 'The Blade' Yurinov","theme":"movies"},

    {"id": 21, "quote":"Oh, I'm sorry, did I break your concentration? ","context":"Pulp Fiction","source":"Jules","theme":"movies"},

    {"id": 22, "quote": "Momentum, a function of mass and velocity, is conserved between portals. In layman's terms, speedy thing goes in, speedy thing comes out.","context":"Portal","source":"GlaDOS","theme":"games"},

    {"id": 23, "quote": "You talkin' to me?","context": "Taxi Driver","source": "Travis Bickle","theme": "movies"},

    {"id": 24, "quote": "Are you not entertained! Are you not entertained! Is this not why you are here!","context": "Gladiator","source": "Maximus","theme": "movies"},

    {"id": 25, "quote": "Here's Johnny","context": "Jack Torrance","source": "The Shining","theme": "movies"},

    {"id": 26, "quote": "Mama always said life was like a box of chocolates. You never know what you're gonna get.","context": "Forest Gump","source": "Forest Gump","theme": "movies"},

    {"id": 27, "quote": "E.T. phone home","context": "E.T.","source": "E.T. The Extra-Terrestrial","theme": "movies"},

    {"id": 28, "quote": "Toto, I've got a feeling we're not in Kansas anymore","context": "Dorothy","source": "The Wizard of Oz","theme": "movies"},

    {"id": 29, "quote":"Open the pod bay doors, please, HAL","context":"2001: A Space Odyssey","source":"Dave","theme":"movies"},

    {"id": 30, "quote":"I'm not bad. I'm just drawn that way.", "source":"Jessica Rabbit", "context":"Who Framed Roger Rabbit", "theme":"movies"},

    {"id": 31, "quote":"When I first saw you, I thought you were handsome. Then, of course, you spoke.", "source":"Carol", "context":"As Good As It Gets", "theme":"movies"},

    {"id": 32, "quote":"Listen, here's the thing. If you can't spot the sucker in your first half hour at the table, then you ARE the sucker.", "source":"Mike", "context":"Rounders", "theme":"movies"},

    {"id": 33, "quote":"The cake is a lie","context":"Portal","source":"Corpse","theme":"games"},

    {"id": 34, "quote":"Welcome, everybody, to Monday Night Combat! We'd like to remind fans that we're committed to creating a safe, comfortable, enjoyable experience for only our Club-level and VIP guests. Everybody else...pay up for better seats next time!", "context":"Monday Night Combat", "source": "Mickey", "theme":"games"},

    {"id": 35, "quote":"Good men mean well. We just don't always end up doing well", "context":"Dead Space 3", "source": "Isaac", "theme":"games"},

    {"id": 36, "quote":"The next time you raise a hand to me will be the last time you have hands", "context":"Game of Thrones", "source":"Khaleesi","theme":"movies"},

    {"id": 37, "quote":"I'm not in the meth business. I'm in the empire business", "context":"Breaking Bad", "source":"Walter","theme":"movies"},

    {"id": 38, "quote":"If you don't like what's being said, change the conversation", "context":"Mad Men", "source":"Don Draper","theme":"movies"},
    
    {"id": 39, "quote":"See that thing on my belt? Grab it! Whatever you do, don’t let go.","context":"Batman", "source":"Batman","theme":"movies"}
  ] 
  }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
