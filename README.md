## TCAD Coding Challenge and Answers

a.	What is the purpose of this application, where is the data it uses pulled from, and what application features are important for someone looking at the code to understand?

    Purpose: allows users to filter through data from robohash api that return a json payload with information about each robot.
    Data is pulled form robohash's api
    Application features: each component is simple to understand. They were broken down to the simplest form and work together to build this app.

b.	What are some good ways to us passwords, keys, etc. in your applications while preventing them from being accessed by the outside world?
    
    They need to be encrypted before being saved in a database. Usually what you do is that you use an algorithm that cannot be reversed.
    Usually when you encode stuff, you need to add a hash key, or an encryption key
    and that key you always use it for encoding
    if the key changes, the encoding for the same password will be different

c.	Your favorite SQL database includes tables called properties and addresses.
- The properties table has one record per property, and has 2,000 records in it.
- The properties table has one column only: prop_id.
- The addresses table has one record per property, per year, and has 500,000 records in it.
- The addresses table has three columns: prop_id, address, and year.
- The year column is comprised of integer values for each year (2010, 2011, and so on)

What is a SQL query that will pull all of the prop_id’s and current (2019) addresses for any property in the addresses table, along with a column denoting whether that property exists in the properties table?

    
    select prop_id, address, (select ) as exists from addresses where year = 2019;
    not quite sure about this one.

d.	What are some cases for or against containerization of internally-used micro-applications?
    For: 
        Continuous Deployment and Testing, Rapid Deployment, Simplicity and Faster Configurations, Compatibility and Maintainability, and efficiency
    Against: 
        Security, Isolation, Networking, Containers add more cost than you expect.





This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
