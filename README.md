# Creating Stock Dashboard Web Application (Stockie)

## IDE
1. Microsoft Visual Code

<details>
  <summary>Required technology:</summary>
  <p>
    <ul>
      <li>
        NodeJS: Development environment
      </li>
      <li>
        ReactJS: UI library
      </li>
      <li>
        Typescript: Superset of Javascript
      </li>
      <li>
        Ant Design: UI framework
      </li>
      <li>
        Axios: Making API calls
      </li>
      <li>
        Config: Handling environment configuration
      </li>
      <li>
        Alpha Vantage: Stock data API provider
      </li>
      <li>
        create-react-app: ReactJS bundler
      </li>
      <li>
        JOI: Data validation
      </li>
      <li>
        nodemon: NodeJS Monitor
      </li>
      <li>
        Express: Web application framework
      </li>
      </li>
    </ul>
  </p>
</details>

## Optional technology:
1. MongoDB: NoSQL database
2. Mongoose: Connector to MongoDB

## Tips:
1. To minimise typing errors, I recommend copying the CMD commands from this tutorial into your CMD.

## 1. Setting up
### 1(a). Downloading NodeJS
### 1(b). Create a react app with create-react-app

To ensure maximum compatibility between the tutorial and the project on your computer, I recommend that you create the directories according to how it is in the tutorial. I have put the entire project in the following directory ```C:/node```. If you have __not__ got the same directory structure, please make one via Window Explorer or Command Prompt (CMD). Throughout this tutorial series, a lot of the navigation will be done through CMD and VS Code built-in command line tool.

Open CMD
To create the ```C:/node``` directory, in the CMD, type: 

> ```mkdir node && cd node```

To start a new Create React App project with Typescript, we will run the following command:

> ```npx create-react-app stockie --template typescript```

*__Note__: If you've previously installed ```create-react-app``` globally via ```npm install -g create-react-app```, the Create React App developers recommend that you uninstall the package using ```npm uninstall -g create-react-app``` to ensure that ```npx``` always uses the latest version because global installs of ```create-react-app``` are no longer supported.*

As we will be working with Typescript, we will also need to install it. Firstly, we will navigate into our newly created app directory via CMD with the command:

> ```cd stockie```

Let's install Typescript;

> ```npm install --save typescript @types/node @types/react @types/react-dom @types/jest```

Let's open VS Code from Stockie's directory with the following command

> ```code .```

After installations, the files with the ```.jsx``` extensions should be automatically renamed to ```.tsx```. If __not__, please renamed the file extension.

## 2. Developing the back-End
### 2(a). Server setup with NodeJS
### 2(b). Setting up endpoints
### 2(c). Connecting to Alpha Vantage
### 2(d). Sending requests to Alpha Vantage

## 3. Developing the front-End

### Cleaning up ```create-react-app```

When we open the project at the root directory, ```create-react-app``` would have created three directories:
1. ```node_modules```
2. ```public```
3. ```src```

Let's start our React app with the following CMD command:

> ```npm start```

This should automatically create a server on a free port, usually port 3000 unless it's being used.

The ```create-react-app``` library helps us to bootstrap our React app. It is very convenient but there are a few things we do __not__ need for this project. So let's get rid of them.

The ```src``` folder is where we have all our React components. Let's open the ```App.tsx``` file in the ```src``` folder and get rid of a few lines of codes. We should have the following lines of codes in our ```App.tsx``` file.

```
import React, { Component } from "react";
import "./App.css";

export default class App extends Component {
	render() {
		return <div></div>;
	}
}
```

We can delete the ```App.css``` and the ```logo.svg``` files for now to declutter our ```src``` folder. At the same time, we can delete everything in the ```index.css``` file.

### 3(a). Installing ```antd```
Ant design (```antd```) is a React Design Framework. It offers a set of high quality components and demos for building rich, interactive user interfaces. In order to use its API we need to install it.

In our project root directory, run the following CMD command:
> ```npm install antd```

### 3(b). Testing ```antd```
Let's do a quick test to see if ```antd``` was correctly installed.

In our ```App.tsx```, let's create an ```antd``` Button component. We can name import it with the following line of code:

> ``` import {Button} from "antd"```

Then we will create the Button component in our ```div``` element and give it the type of ```primary```. Our ```App.tsx``` should look like this:

```
import React, { Component } from "react";
import { Button } from "antd";
import "./App.css";

export default class App extends Component {
render() {
	return (
		<div>
			<Button type="primary">Primary Button</Button>
		</div>
		);
	}
}
```

Once we save the file, our server should auto-reload. If we look at our application, it should show a stock-standard HTML button. This looks boring and is rather unwhelming. The reason for this lack of styling is that we have yet to import in the ```antd``` css file. So let's do this.

Go into the ```index.css``` file and type the following line of code:

> ```@import "~antd/dist/antd.css;"```

Save the file and let's check out our application now. Voila! We have styles!

### 3(c). Configuring ```antd```
#### 3(c)(1). What is ```Webpack```?
At its core, ```webpack``` is a *static module bundler* for modern Javascript applications. When webpack processes your application, it internally builds a dependency graph which maps every module your project needs and generates one or more bundles. ([source](https://webpack.js.org/concepts/))

### 3(a). Create navbar
### 3(b). Create drawer
### 3(c). Create graph
### 3(d). Connecting to back-end

## 4. Final Touches
### 4(a). Handling secrets and authentication

## 5. Extra Extra: Creating accounts with MongoDB
### 5(a). Setting up a MongoDB account
### 5(b). Installing mongoose
### 5(c). Setting up endpoints
### 5(d). Data validation
### 5(e). Connecting front-end to back-end

## 6. Glossary
* CMD: Command Prompt
* (project) root directory: ```C:/node/stockie```
