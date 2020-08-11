# React Tutorial

See [React Tutorial](https://reactjs.org/tutorial/tutorial.html) for details.

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## How to embed this app into any site

See [this article](https://medium.com/better-programming/how-to-embed-a-react-application-on-any-website-1bee1d15617f) 
for details.

1. Change the app target div to something unique instead of `root`, e.g. `myJsTutorialRoot`:
    ```javascript
    ReactDOM.render(
        <Game/>,
        document.getElementById('myJsTutorialRoot')
    );
    ```
1. Add `.` homepage to `package.json`:
    ```json
    {
      "name": "reactjs-tutorial",
      "version": "0.1.0",
      "private": true,
      "homepage": ".",
      "...": "..."
    }
    ```
1. Build the app: `npm run build`
1. Create an HTML page:
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
      <title>React App</title>
    
      <style>
        <!-- CSS styles content -->
      </style>
    </head>
    <body>
    
      <div id="myJsTutorialRoot"></div>
      
      <script type="text/javascript">
        <!-- runtime-main.(hash).js content -->
      </script>
      <script type="text/javascript">
        <!-- 2.(hash).chunk.js content -->
      </script>
      <script type="text/javascript">
        <!-- main.(hash).chunk.js content -->
      </script>
    
    </body>
    </html>
    ``` 
1. Include CSS styles content into the HTML page
1. Include the following JS contents into the HTML page (**the order does matter!**):
    * `build/static/js/runtime-main.(hash).js`
    * `build/static/js/2.(hash).chunk.js`
    * `build/static/js/main.(hash).chunk.js`
1. Embed resulting HTML into the target site


## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
