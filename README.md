# px-path-guide
[![Build Status](https://travis-ci.org/PredixDev/px-path-guide.svg?branch=master)](https://travis-ci.org/PredixDev/px-path-guide)

## Custom Styles

--px-path-guide-connector-length: 120px;
--px-path-guide-border-size: 2px;

### Default Step Styles
--px-path-guide-step-diameter: 20px;
--px-path-guide-step-border-radius: 10px;
--px-path-guide-step-border-color: $gray4;
--px-path-guide-step-fill-color: $gray3;
--px-path-guide-connector-color: $gray4;

### Default Icon Styles
--px-path-guide-icon-size: 14px;
--px-path-guide-icon-color: #333;

### Step Label Styles
--px-path-guide-step-label-font-size: 15px;
--px-path-guide-step-label-font-weight: normal;
--px-path-guide-step-label-color: $black;

### 'Current' State Styles
--px-path-guide-current-step-diameter: 24px;
--px-path-guide-current-step-border-radius: 12px;
--px-path-guide-current-step-border-color: $select-blue-default;
--px-path-guide-current-step-fill-color: $white;
--px-path-guide-current-connector-color: $select-blue-default;

### 'Current' Icon Styles
--px-path-guide-current-icon-size: 14px;
--px-path-guide-current-icon-color: $select-blue-default;

### 'Current' Label Styles
--px-path-guide-current-step-label-color: $black;
--px-path-guide-current-step-label-font-weight: bold;

### 'Complete' State Styles
--px-path-guide-complete-step-diameter: 20px;
--px-path-guide-complete-step-border-radius: 10px;
--px-path-guide-complete-step-border-color: $select-blue-default;
--px-path-guide-complete-step-fill-color: $white;
--px-path-guide-complete-connector-color: $select-blue-default;

### 'Complete' Icon Styles
--px-path-guide-complete-icon-size: 14px;
--px-path-guide-complete-icon-size: 14px;
--px-path-guide-complete-icon-color: $select-blue-default;

### 'Complete' Label Styles
--px-path-guide-complete-step-label-color: $black;
--px-path-guide-complete-step-label-font-weight: normal;

### Path Label Styles
--px-path-guide-path-label-margin-right: 20px;
--px-path-guide-path-label-color: #333;
--px-path-guide-path-label-font-size: 12px;

px-path-guide is a Polymer web component that is a visual representation of any sequence of steps and progress made on those steps.  It can show which steps have been completed, the current step, and remaining steps, for example.  Its visual details (nodes, connecting lines, icons, fonts, etc.) can be styled using custom CSS properties (shown in red in the above diagram).

## Overview

Use the px-path-guide to represent any sequence of steps in a process.  An example of a process is user account creation, which can consist of this sequence of steps: 1. Sign Up, 2. Email Confirmation, 3. Account Activation and 4. Account Configuration.  px-path-guide can represent this process with a sequence of nodes (circles by default) corresponding to the steps.  Each step is labeled accordingly.  px-path-guide can place connector lines between adjacent steps.  Each step's completion state can be symbolized by a font-awesome icon, like a checkmark ('fa-check') for a completed step.

## Usage

### Prerequisites
1. node.js
2. npm
3. bower
4. Install the [webcomponents-lite.js polyfill](https://github.com/webcomponents/webcomponentsjs) to add support for web components and custom elements to your application.

### Getting Started

First, install the component via bower on the command line.

```
bower install px-path-guide --save
```
Second, import the component to your application with the following tag in your head.

```
<link rel="import" href="/bower_components/px-path-guide/px-path-guide.html"/>
```

Finally, use the component in your application:

```
<px-path-guide></px-path-guide>
```

<br />
<hr />

## Documentation

Read the full API and view the demo [here](https://predixdev.github.io/px-path-guide).

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

Please use [Github Issues](https://github.com/PredixDev/px-path-guide/issues) to submit any bugs you might find.
