
REDUX ::: THREE PRINCIPLES

Redux is a state management tool . Whenever your application is growing in such a way that one single is having three or more child components in a chain format.

Parent.js <- Child1.js <- Child2.js <- Child3.js

Just imagine you have any data(present in parent) which is used only in Parent.js and Child3.js . But based on above structure we will have to pass the data in Child1 and Child2 as well where this data is not even required.

Three principles :

1> SSOT : single source of truth. All the state variables that is required to be shared with multiple component that will be kept inside the store of redux.

2> Action : Every action has a change in state. If you want to update the state variable value which is present in redux store then you can not update by using setState or useState hook . You will have to pass or fire an action to update the state variable value. This also contains action types (uppercase letter) , this helps to understand that at which action type what action has to be fired.

3> Pure Function : Reducer : Reducer is a pure function. To update the state variable value we need to return the action type and new value of state from action. This will automatically come to the respective reducer function , this function takes in two param i.e. state , action . Since it is a pure function so the state object which it receives as a param it will not update that value , instead of it will return you the new state object.

mapStateToProps / useSelector : helps to connect with state of the redux store and component

mapDispatchToProps / useDispatch : helps you to connect with what actions you have to fire.

connect

createStore

combineReducer

Complete application should be wrapped with Provider component

redux react-redux





# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
