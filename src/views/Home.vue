<template>
  <div class="home">
   <div class="main">
    <div class="text-box">
      <p style="font-size: 15.5vw; margin:7vw 0 0 0;" id="saad">SAAD</p>
      <p style="font-size: 5vw; margin:-4vw 9vw 0 0;" id="ul">ul</p>
      <p style="font-size: 10vw; margin:-5.5vw 0 0 25vw;" id="kabir">KABIR</p>
    </div>
	<div class="wrapper">
		<div class="button">
			<div class="icon">
				<fa icon="instagram" />
			</div>
			<span>Instagram</span>
		</div>

		<div class="button">
			<div class="icon">
				<i class="fab fa-facebook-f"></i>
			</div>
			<span>Facebook</span>
		</div>

		<div class="button">
			<div class="icon">
				<i class="fab fa-twitter"></i>
			</div>
			<span>Twitter</span>
		</div>

		<div class="button">
			<div class="icon">
				<i class="fab fa-linkedin"></i>
			</div>
			<span>LinkedIn</span>
		</div>

		<div class="button">
			<div class="icon">
				<i class="fab fa-youtube"></i>
			</div>
			<span>YouTube</span>
		</div>

		<div class="button">
			<div class="icon">
				<i class="fab fa-github"></i>
			</div>
			<span>Github</span>
		</div>
	</div>
   </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    // HelloWorld
  }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Righteous&display=swap');
#saad {
  background: -webkit-linear-gradient(rgb(255, 251, 0), rgb(255, 136, 0));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
#ul {
  background: -webkit-linear-gradient( rgb(255, 255, 255), rgb(87, 87, 87));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  
}
#kabir {
  background: -webkit-linear-gradient(rgb(255, 251, 0), rgb(255, 136, 0));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.text-box {
font-family: 'Righteous', cursive;
}
.main {
    position:absolute;
    top:0;
    left:0;
    bottom:0;
    right:0;
    height:100%;
    width:100%;
    backdrop-filter: blur(10px) saturate(90%);
    color: #ffffff;
    
}
body {
  height: 100%;
  --s: 25vmin;
  --p: calc(var(--s) / 2);
  --c1: rgb(48, 46, 54);
  --c2: rgb(36, 34, 41);
  --c3: rgb(24, 23, 27);
  --bg: var(--c3);
  --d: 4000ms;
  --e: cubic-bezier(0.76, 0, 0.24, 1);

  
  
  background-color: var(--bg);
  background-image:
    linear-gradient(45deg, var(--c1) 25%, transparent 25%),
    linear-gradient(-45deg, var(--c1) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, var(--c2) 75%),
    linear-gradient(-45deg, transparent 75%, var(--c2) 75%);
  background-size: var(--s) var(--s);
  background-position: 
    calc(var(--p) *  1) calc(var(--p) *  0), 
    calc(var(--p) * -1) calc(var(--p) *  1), 
    calc(var(--p) *  1) calc(var(--p) * -1), 
    calc(var(--p) * -1) calc(var(--p) *  0);
  animation: 
    color var(--d) var(--e) infinite,
    position var(--d) var(--e) infinite;
}

@keyframes color {
  0%, 25% {
    --bg: var(--c3);
  }
  26%, 50% {
    --bg: var(--c1);
  }
  51%, 75% {
    --bg: var(--c3);
  }
  76%, 100% {
    --bg: var(--c2);
  }
}

@keyframes position {
  0% {
    background-position: 
      calc(var(--p) *  1) calc(var(--p) *  0), 
      calc(var(--p) * -1) calc(var(--p) *  1), 
      calc(var(--p) *  1) calc(var(--p) * -1), 
      calc(var(--p) * -1) calc(var(--p) *  0);
  }
  25% {
    background-position: 
      calc(var(--p) *  1) calc(var(--p) *  4), 
      calc(var(--p) * -1) calc(var(--p) *  5), 
      calc(var(--p) *  1) calc(var(--p) *  3), 
      calc(var(--p) * -1) calc(var(--p) *  4);
  }
  50% {
    background-position: 
      calc(var(--p) *  3) calc(var(--p) * 8), 
      calc(var(--p) * -3) calc(var(--p) * 9), 
      calc(var(--p) *  2) calc(var(--p) * 7), 
      calc(var(--p) * -2) calc(var(--p) * 8);
  }
  75% {
    background-position: 
      calc(var(--p) *  3) calc(var(--p) * 12), 
      calc(var(--p) * -3) calc(var(--p) * 13), 
      calc(var(--p) *  2) calc(var(--p) * 11), 
      calc(var(--p) * -2) calc(var(--p) * 12);
  }
  100% {    
    background-position: 
      calc(var(--p) *  5) calc(var(--p) * 16), 
      calc(var(--p) * -5) calc(var(--p) * 17), 
      calc(var(--p) *  5) calc(var(--p) * 15), 
      calc(var(--p) * -5) calc(var(--p) * 16);
  }
}

@media (prefers-reduced-motion) {
  body {
    animation: none;
  }
}

.button {
	float: left;
	width: 60px;
	height: 60px;
	cursor: pointer;
	background: #fff;
	overflow: hidden;
	border-radius: 50px;
	transition: all 0.3s ease-in-out;
	box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);
}

.button span {
	font-size: 20px;
	font-weight: 500;
	line-height: 60px;
	margin-left: 10px;
}

.button:hover {
	width: 200px;
}

.button:nth-child(1):hover .icon {
	background: #e1306c;
}

.button:nth-child(2):hover .icon {
	background: #4267b2;
}

.button:nth-child(3):hover .icon {
	background: #1da1f2;
}

.button:nth-child(4):hover .icon {
	background: #0e76a8;
}

.button:nth-child(5):hover .icon {
	background: #ff0000;
}

.button:nth-child(6):hover .icon {
	background: #333;
}

.button:nth-child(1) span {
	color: #e1306c;
}

.button:nth-child(2) span {
	color: #4267b2;
}

.button:nth-child(3) span {
	color: #1da1f2;
}

.button:nth-child(4) span {
	color: #0e76a8;
}

.button:nth-child(5) span {
	color: #ff0000;
}

.button:nth-child(6) span {
	color: #333;
}

.button .icon {
	width: 60px;
	height: 60px;
	text-align: center;
	border-radius: 50px;
	display: inline-block;
	transition: all 0.3s ease-in-out;
}

.button .icon i {
	font-size: 25px;
	line-height: 60px;
	transition: all 0.3s ease-in-out;
}

.button:hover i {
	color: #fff;
}

</style>
