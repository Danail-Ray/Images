<template>
  <head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
  </head>

  <div class="container">
  <div>
    <h1> Shop with Dancholini</h1>
  </div>
</div>

  <div class="card">
    <div class="card-content">
          <h2 class="pulsating-text"> Get your new Acc here!  </h2>
    </div>
  </div>

  <div class="icons">
    <a href="https://discord.com/invite/your-discord-invite-link" target="_blank">
      <i class="fab fa-discord"></i>
    </a>
    <a href="https://www.instagram.com/your-instagram-profile" target="_blank">
      <i class="fab fa-instagram"></i>
    </a>
    <a href="https://www.twitter.com/your-instagram-profile" target="_blank">
      <i class="fab fa-twitter"></i>
    </a>
  </div>

 </template>

<script>
export default {
  name: "App",
  data () {
    return {
    
    }
  },

  methods: {
  
  },
};
</script>

<style>

.lol-image {
  width: 300px; /* Adjust the width as needed */
  height: auto; /* Automatically adjust the height to maintain aspect ratio */
  border: 2px solid #333; /* Add a border */
  border-radius: 10px; /* Add rounded corners */
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5); /* Add a shadow */
  margin: 10px; /* Add margin for spacing */
  display: block; /* Make the image a block element */
  margin-left: auto; /* Center the image horizontally */
  margin-right: auto;
}

@keyframes shake {
  0% {
    transform: translateX(0);
  }
  25% {
    transform: translateX(-5px); /* Adjust the shake intensity */
    transform: translateY(-5px)
  }
  50% {
    transform: translateX(5px); /* Adjust the shake intensity */
    transform: translateY(5px)

  }
  75% {
    transform: translateX(-5px); /* Adjust the shake intensity */
    transform: translateY(-5px)
  }
  101% {
    transform: translateX(5px); /* Adjust the shake intensity */
    transform: translateY(5px)
  }
}

.shaking-text {
  animation: shake 2s ease-in-out 10s infinite; /* Shake animation every 3 seconds */
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh; /* Adjust the height as needed */
}

:root {
  --card-color: linear-gradient(180deg, rgba(2,0,36,1) 0%, rgba(198,49,153,1) 0%, rgba(0,212,255,1) 100%); 
}

#cards {
  display: grid;
  gap: 1em;
  max-width: 1000px;
  padding: 1em 0em;
  position: relative;
  width: calc(100% - 2em);
  z-index: 2;
}

.card {
  background-color: var(--card-color);
  border-radius: 0.75em;
  cursor: pointer;
  height: 120px;
  position: relative;
  background-image: none;
}

.card:hover:before {
  opacity: 1;
}

.card:before {
  background: linear-gradient(
    40deg,
    transparent 5%,
    rgba(198,49,153,1) 50%,
    transparent 98%
  );
  border-radius: inherit;
  content: "";
  inset: 0px;
  opacity: 0;
  position: absolute;
  transition: opacity 400ms;
  z-index: 0%;
  border: 1px solid #ccc;
  border-radius: 4px;
}

.card-content {
  background-color: var(--card-color);
  border-radius: inherit;
  display: contents;
  inset: 1px;
  padding: 1em;
  position: absolute;

  text-align: center; /* Center text horizontally */
  display: flex; /* Create a flex container */
  justify-content: center; /* Center content horizontally within the flex container */
  align-items: center; /* Center content vertically within the flex container */
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
 /* text-align: center;*/
  color: #2c3e50;
  margin-top: 60px;
}

.underline{
  text-decoration: underline;
}

.promoted{
  font-style: italic;
}

h1 {
  font-size: 3rem; /* Adjust the font size as needed */
  font-family: 'Roboto', sans-serif; /* Use a desired font-family */
  color: #46e2da; /* Text color */
  text-transform: uppercase; /* Convert text to uppercase */
  letter-spacing: 2px; /* Increase letter spacing for emphasis */
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3); /* Add a subtle text shadow */
  background: linear-gradient(45deg, #000000, #1132d2); /* Gradient background */
  -webkit-background-clip: text; /* Clip the background to text */
  background-clip: text;
  -webkit-text-fill-color: transparent; /* Make text transparent to show the background */
  padding-left: 20px; /* Adjust as needed */
  padding-right: 20px; /* Adjust as needed */
}

.icons {
  position: absolute;
  display: flex;
  gap: 5px;
  bottom: 0;
  left: 0;
  margin: 10px; /* Optional margin to provide spacing */
}

@keyframes pulse {
  0% {
    opacity: 1;
    transform: scale(1);
  }
  50% {
    opacity: 1;
    transform: scale(1.1);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}

.pulsating-text {
  font-size: 34px; /* Adjust the font size as needed */
  color: #000000; /* Text color */
  animation: pulse 2s infinite; /* Apply the pulse animation */
  
}

.delayed-text {
  display: none; /* Initially hide the text */
  font-size: 24px; /* Adjust the font size as needed */
  color: #c80b0b; /* Text color */
  animation: fadeIn 1s 3s forwards; /* Apply fade-in animation after 5 seconds */
}

@keyframes fadeIn {
  to {
    display: block; /* Change the display property to 'block' to show the text */
    opacity: 1; /* Fade in the text */
  }
}

label {
  font-weight: bold;
  display: flex;
  margin-bottom: 6px;
  margin-left: 4px;
}

input {
  font-weight: lighter;
  margin-bottom: 20px;
}

input + label {
  font-weight: lighter;
  display: contents;
  margin-left: 20px;
}

body {
  margin: 0;
  height: 60vh;
  display: flex;
  justify-content: center;
  align-items: center;
  
  background: rgb(2,0,36);
  background: linear-gradient(180deg, rgba(2,0,36,1) 0%, rgba(198,49,153,1) 0%, rgba(0,212,255,1) 100%); 
  background-attachment: fixed;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
}

input[type='text'],
textarea,
select{
  display: block;
  width: 400px;
  padding: 6px 12px;
  font-size: 14px;
  line-height: 1.43857143;
  color: #555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 4px;
  
}
</style>
