# Guaranteed Less Loss =)
Angular Material module Confirm form loss

![IMG](https://coverfiles.alphacoders.com/357/35762.jpg)

<p>
  <a href="https://gitter.im/miamarti/mdFormConfirm?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge" target="_blank"><img src="https://badges.gitter.im/Join%20Chat.svg"></a>
  <a href="https://gitlab.com/miamarti/mdFormConfirm" target="_blank"><img src="https://img.shields.io/badge/gitlab-mdFormConfirm-yellow.svg"></a>
  <img src="https://img.shields.io/badge/mdFormConfirm-release-green.svg">
  <img src="https://img.shields.io/badge/version-1.4.0-blue.svg">
  <img src="https://img.shields.io/github/license/mashape/apistatus.svg">
  <a href="https://github.com/miamarti/mdFormConfirm/tarball/master"><img src="https://img.shields.io/npm/dt/md-form-confirm.svg"></a>
</p>

[on npm](https://www.npmjs.com/package/md-form-confirm)

### Dependencies
Download make the dependencies of mdFormConfirm and include in your project
* https://angularjs.org/
* https://material.angularjs.org/latest/

### Installation
```
$ npm install md-form-confirm --save
```

### Result
![IMG](https://i.imgur.com/SDykKl8.png)

### Module AngularJS include
```
require('angular');

angular.module('Requisition', [
  require('angular-animate'),
  require('angular-material'),
  require('md-form-confirm') //Component Injection
])
```

## Implementation
```
<form name="joyForm" ctrl="prettyCrazyController" obj="model" native-confirm="true" form-control="prettyCrazyController.enableConfirm" ng-submit="prettyCrazyController.save()">
  <input name="code" ng-model="prettyCrazyController.model.code">
  <md-button type="submit" ng-disabled="!joyForm.$valid || !joyForm.$isChanged()">SAVE</md-button>
</form>
```

## Parameters

| Name  | Type   | Dinamic | Mandatory | Description                                           |
| ------| ------ | ------- | --------- | ----------------------------------------------------- |
| name  | String | false   | true      | Form Name                                             |
| ctrl  | String | false   | true      | Controller Name                                       |
| obj   | String | false   | true      | Name of the model object (assigned to the form)       |
| native-confirm | Boolean | true | false | Put a validation message on the screen preventing the screen from being reloaded |
| form-control | Boolean | true | true | Controls wether the feature will be on or off |
| form-confirm-reject | Function | true | false | Binds function to be executed if confirmation popup gets canceled |
| $isChanged  | Method | true   | false      | Method assigned to the form, tells if it has been changed (can be accessed in the view) |
| $updateChanged  | Method | true   | false      | Method that updates the status of unmodified form |



## Development
Edit `version.js` and run the command below:

```
$ npm run build
```

## Metrics

[![Throughput Graph](https://graphs.waffle.io/miamarti/mdFormConfirm/throughput.svg)](https://waffle.io/miamarti/mdFormConfirm/metrics/throughput)
