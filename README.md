# @pera-swarm/modes

[![npm (scoped)](https://img.shields.io/npm/v/@pera-swarm/modes.svg)](https://github.com/Pera-Swarm/modes/)
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Pera-Swarm/modes/%F0%9F%9A%80%20Release)
[![GitHub issues](https://img.shields.io/github/issues/Pera-Swarm/modes)](https://github.com/Pera-Swarm/modes/issues)

# Install

```
$npm install --save @pera-swarm/modes
```

# Usage

```
const { Mode } = require('@pera-swarm/modes');

const exampleSetup = () => {
    console.log('setup fn');
};

const exampleFlow = () => {
    console.log('flow fn');
};

new Mode(exampleSetup, exampleFlow, 10000, 'server-mode').start();
```

or

```
const { defineBaseMode } = require('@pera-swarm/modes');

const exampleSetup = () => {
    console.log('setup fn');
};

const exampleFlow = () => {
    console.log('flow fn');
};

defineBaseMode(exampleSetup, exampleFlow);
```

or

```
const { start } = require('@pera-swarm/modes');

const exampleSetup = () => {
    console.log('setup fn');
};

const exampleFlow = () => {
    console.log('flow fn');
};

start(exampleSetup, exampleFlow, 1000, 'my-custom-mode');
```
