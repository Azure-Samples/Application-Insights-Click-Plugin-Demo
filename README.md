# Application Insights JS with Click Analytics Plugin - HTML sample

This is a simple HTML/CSS/JS web app that illustrates how to enable Application Insights Click Analytics Plugin

It is built on the [Carousel template](http://getbootstrap.com/examples/carousel) by [Bootstrap](http://getbootstrap.com).

## Pre-requisites 

1. [Git](https://docs.microsoft.com/en-us/azure/devops/learn/git/install-and-set-up-git) and [Node.js](https://docs.microsoft.com/en-us/windows/nodejs/setup-on-windows) installed on your computer.
2. Familiarity with editing text and code files in any text editor.

## Get Started

1.  Create an Application Insights resource in Azure by following [these instructions](https://docs.microsoft.com/en-us/azure/application-insights/app-insights-javascript?toc=/azure/azure-monitor/toc.json).

2.  Open terminal and clone the repo using `git clone` 

3.  Grab the Instrumentation Key (aka "ikey") from the resource you created in step 1. Later, you'll add it to the instrumentationKey setting in the `public/ts/appinsights.ts` file

4.  In the project directory you should run `npm install` on your terminal to install all the dependencies.

5.  After making the changes in step-3, please run `npm run build` on your terminal to transpile and browserify the `appinsights.ts` file

6.  To launch the app locally , simply run the following command on your terminal

    `node index.js`

7. 	Open your favorite browser and go to http://localhost:8000/


## Correlating HTML tags with telemetry data.

### How to see the telemetry data generated from client side?

1. In the same tab where you have the sample app running, open the 'Developer tools' and go to 'Network' tab.
2. Start clicking different navigation buttons like 'Home', 'About' etc.
3. After around 15s, you should see 'track' events in the network tab as shown below.

:::image type="content" source="doc-img/networktab.png" alt-text="Screenshot of the Network Tab.":::