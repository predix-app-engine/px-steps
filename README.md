# px-steps
[![Build Status](https://travis-ci.org/PredixDev/px-steps.svg?branch=master)](https://travis-ci.org/PredixDev/px-steps)

px-steps is a Polymer web component that is a visual representation of any sequence of steps and progress made on those steps. It can show which steps have been completed, the current step, and remaining steps, for example.

## Overview

Use the px-steps to represent any sequence of steps in a process.  An example of a process is user account creation, which can consist of this sequence of steps: 1. Sign Up, 2. Email Confirmation, 3. Account Activation and 4. Account Configuration.  px-steps can represent this process with a sequence of nodes corresponding to the steps.  Each step is labeled accordingly.  px-steps can place connector lines between adjacent steps.

## Usage

### Prerequisites
1. node.js
2. npm
3. bower
4. Install the [webcomponents-lite.js polyfill](https://github.com/webcomponents/webcomponentsjs) to add support for web components and custom elements to your application.

### Getting Started

First, install the component via bower on the command line.

```
bower install px-steps --save
```
Second, import the component to your application with the following tag in your head.

```
<link rel="import" href="/bower_components/px-steps/px-steps.html"/>
```

Finally, use the component in your application:

```
<px-steps items='[{ id: "1", label: "Select Services"},{ id: "2", label: "Billing"}]'></px-steps>
```

<br />
<hr />

## Documentation

Read the full API and view the demo [here](https://www.predix-ui.com/#/elements/px-steps).

## Using Events

Events follow the [Polymer data-binding standards](https://www.polymer-project.org/1.0/docs/devguide/data-binding.html).

You can can attach the following listener(s) to these parts of the component:

1. Mouseclick event on a step.
<br />
<hr />

## Local Development

From the component's directory, to setup the component and its dependencies:

```
$ npm install
$ bower install
$ gulp sass
```

From the component's directory, to start a local server and automatically bring up web page of the component demo:

```
$ gulp serve
```

(A web page with URL http://localhost:8080/ will be opened in your default browser.)

### LiveReload

By default gulp serve is configured to enable LiveReload and will be watching for modifications in your root directory as well as `/css`.

### GE Coding Style Guide
[GE JS Developer's Guide](https://github.com/GeneralElectric/javascript)

<br />
<hr />

## Known Issues

Please use [Github Issues](https://github.com/PredixDev/px-steps/issues) to submit any bugs you might find.
