# Props-Assignment-1

# Develop the simple applicaiton by using props in ReactJS.
## The following is the screenshort to implement:

![image](https://user-images.githubusercontent.com/128453440/226533080-1940d801-2ee8-408c-ab45-3444814a829f.png)


### In order to implement the above requirement we need to following below steps:
##Step1: Create the React Application

##Step2: Open the project inside the visual studio.

##Step3: Under Src folder create Components folder

##Step4: Under the Components folder create the following two components:

             - Working.js

             - Car.js
##Step5: The following is the code inside the Working.js file

```
import React, { Component } from 'react'
import Car from './Car';
export class Working extends Component {
    
    render() {
     const cars=['Ford','BMW','Audi'];
    return (
      <div>
            <h2>The following are the Cars:</h2>
            <ul>
                {cars.map((car)=><Car brand={car}/>)}
            </ul>
      </div>
    )
  }
}

export default Working

```

##Step6: The following is the code inside the Car.js file


```
import React, { Component } from 'react'

export class Car extends Component {
  render(props) {
    return (
      <li>I am a {this.props.brand}</li>
    )
  }
}

export default Car
```

##Step7: The following is the code inside the App.js file

```

import React, { Component } from 'react'
import { Working } from './Components/Working';

export class App extends Component {
  render() {
    return (
      <div>
          <Working/>
      </div>
    )
  }
}

export default App
```

##Step8: Start the application:
 - npm start
 
