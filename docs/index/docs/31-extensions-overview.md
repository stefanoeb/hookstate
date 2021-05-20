---
id: extensions-overview
title: Plugins system overview
sidebar_label: Overview
---

import { PreviewSample } from '../src/PreviewSample'

> Please, submit pull request if you would like yours plugin included in the list.

## Standard extensions

Plugin | Description | Example | Package | Version
-|-|-|-|-
Initial | Enables access to an initial value of a [State](typedoc-hookstate-core#state) and allows to check if the current value of the state is modified (compares with the initial value). Helps with tracking of *modified* form field(s). | [Demo](./32-extensions-initial) | `@hookstate/initial` | [![npm version](https://img.shields.io/npm/v/@hookstate/initial.svg?maxAge=300&label=version&colorB=007ec6)](https://www.npmjs.com/package/@hookstate/initial)
Touched | Helps with tracking of *touched* form field(s). | [Demo](./34-extensions-touched) | `@hookstate/touched` | [![npm version](https://img.shields.io/npm/v/@hookstate/touched.svg?maxAge=300&label=version&colorB=007ec6)](https://www.npmjs.com/package/@hookstate/touched)
Validation | Enables validation and error / warning messages for a state. Usefull for validation of form fields and form states. | [Demo](./35-extensions-validation) | `@hookstate/validation` | [![npm version](https://img.shields.io/npm/v/@hookstate/validation.svg?maxAge=300&label=version&colorB=007ec6)](https://www.npmjs.com/package/@hookstate/validation)
Persistence | Enables persistence of managed states to browser's local storage. | [Demo](./36-extensions-persistence) | `@hookstate/persistence` | [![npm version](https://img.shields.io/npm/v/@hookstate/persistence.svg?maxAge=300&label=version&colorB=007ec6)](https://www.npmjs.com/package/@hookstate/persistence)
Broadcasted | Enables synchronization of a state across browser tabs. | [Demo](./38-extensions-broadcasted) | `@hookstate/broadcasted` | [![npm version](https://img.shields.io/npm/v/@hookstate/broadcasted.svg?maxAge=300&label=version&colorB=007ec6)](https://www.npmjs.com/package/@hookstate/broadcasted)

## Development tools

Plugin | Description | Example | Package | Version
-|-|-|-|-
DevTools | Development tools for Hookstate. Install [Chrome browser's extension](https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en) and [activate the plugin](./40-devtools-overview) in your app. [Learn more](./40-devtools-overview) about using the development tools. | [Demo](https://hookstate.js.org/demo-todolist) | `@hookstate/devtools` | [![npm version](https://img.shields.io/npm/v/@hookstate/devtools.svg?maxAge=300&label=version&colorB=007ec6)](https://www.npmjs.com/package/@hookstate/devtools)
Logger | Simpler alternative to development tools. Logs state updates and current value of a state to the development console. | | `@hookstate/logger` | [![npm version](https://img.shields.io/npm/v/@hookstate/logger.svg?maxAge=300&label=version&colorB=007ec6)](https://www.npmjs.com/package/@hookstate/logger)

## Special extensions

Plugin | Description | Example | Package | Version
-|-|-|-|-
Labelled | Allows to assign string metadata to a state. | [Demo](./37-extensions-labelled) | `@hookstate/labelled` | [![npm version](https://img.shields.io/npm/v/@hookstate/labelled.svg?maxAge=300&label=version&colorB=007ec6)](https://www.npmjs.com/package/@hookstate/labelled)
Untracked | It allows to get and set a state without triggering rerendering. It also allows to trigger rerendering even when a state has not been updated. You should understand what you are doing if you decide to use this plugin. | [Demo](./25-performance-managed-rendering#untracked-plugin) | `@hookstate/untracked` | [![npm version](https://img.shields.io/npm/v/@hookstate/untracked.svg?maxAge=300&label=version&colorB=007ec6)](https://www.npmjs.com/package/@hookstate/untracked)
Downgraded | Turns off optimizations for a StateLink by stopping tracking of it's value usage and assuming the entire state is *used* if StateLink's value is accessed at least once. | [Docs](./25-performance-managed-rendering) | `@hookstate/core` | [![npm version](https://img.shields.io/npm/v/@hookstate/core.svg?maxAge=300&label=version&colorB=007ec6)](https://www.npmjs.com/package/@hookstate/core)
