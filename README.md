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

After installations, the files with the ```.jsx``` extensions should be automatically renamed to ```.tsx```. If __not__, please renamed the file extension.


### 1(c). Installing Ant Design
### 1(d). Installing Axios
### 1(e). Installing Config
### 1(f). Setting up account with Alpha Vantage

## 2. Developing the back-End
### 2(a). Server setup with NodeJS
### 2(b). Setting up endpoints
### 2(c). Connecting to Alpha Vantage
### 2(d). Sending requests to Alpha Vantage

## 3. Developing the front-End
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
