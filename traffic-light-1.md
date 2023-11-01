# Traffic-Light-1
### First method:

~~~
const trafficLight = {
    state: "green",
  };
  
  let rotations = 0;
  while (rotations < 2) {
    const currentState = trafficLight.state;
    console.log("The traffic light is on", currentState);
  
    // Check the current state and update the traffic light
    if (currentState === "green") {
      trafficLight.state = "orange";
    } else if (currentState === "orange") {
      trafficLight.state = "red";
    } else {
      trafficLight.state = "green";
      rotations++; // Increase the rotation count when it turns red
    }
  }

~~~

### Second method:

~~~
const trafficLight = {
    color: "green",
}

for( let i = 0 ;i < 2 ;  ){
  const colors = trafficLight.color
  console.log(`The traffic light is on ${colors}`);
  if(colors==="green"){
    trafficLight.color = "orang";
  }else if(colors === "orang"){
    trafficLight.color = "red";
  }else{
    trafficLight.color = "green";
    i++
  }
}

~~~

### Third method:

~~~
function trafficLight (...colors){
    for(let i = 0 ; i < colors.length ; i++){
        console.log(`The traffic light is on ${colors[i]}`)
    }
}
console.log(trafficLight("green", "orange", "red","green", "orange", "red"));

~~~
