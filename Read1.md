### Array.map()
 creates a new array by applying some changes to elements of another array, so for example I'd use if I wanted to multiply each element of an array by a number and store the results into a new array.

### Array.reduce() 
converts and array to one element, for example I'd use it if I wanted to find the summation of an array.

### Superagent
Example 1(using then & catch):
```function getLatAndLon(cityName) { superagent .get(url) .then((data) => { let lat = data.body.latt; let lon = data.body.long; console.log(lat, lon); }) .catch((error) => { console.error(error); }); }
Example 2 (using async and await):

async function getLatAndLon (cityName) { let data = await superagent.get(url); let lat = data.body.latt; let lon = data.body.long; console.log(lat, lon): }
```

## #async() / await()
```const https = require('https');
  https.get('https://api.nasa.gov/planetary/apod?api_key=DEMO_KEY', (resp) => {
    let data = '';
    
    // A chunk of data has been received.
    resp.on('data', (chunk) => {
      data += chunk;
    }); 
    
    // The whole response has been received. Print out the result.
    resp.on('end', () => {
      console.log(JSON.parse(data).explanation);
    });
    
  }).on("error", (err) => { 
    console.log("Error: " + err.message);  
  });
  ```


 ### promises
promises is method to tell javascript what to next when finishing an in-bakground job