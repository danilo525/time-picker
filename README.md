# TimePicker

React TimePicker

[![NPM version][npm-image]][npm-url]
[![build status][travis-image]][travis-url]
[![Test coverage][coveralls-image]][coveralls-url]
[![gemnasium deps][gemnasium-image]][gemnasium-url]
[![node version][node-image]][node-url]
[![npm download][download-image]][download-url]

[npm-image]: http://img.shields.io/npm/v/rc-time-picker.svg?style=flat-square
[npm-url]: http://npmjs.org/package/rc-time-picker
[travis-image]: https://img.shields.io/travis/react-component/time-picker.svg?style=flat-square
[travis-url]: https://travis-ci.org/react-component/time-picker
[coveralls-image]: https://img.shields.io/coveralls/react-component/time-picker.svg?style=flat-square
[coveralls-url]: https://coveralls.io/r/react-component/time-picker?branch=master
[gemnasium-image]: http://img.shields.io/gemnasium/react-component/time-picker.svg?style=flat-square
[gemnasium-url]: https://gemnasium.com/react-component/time-picker
[node-image]: https://img.shields.io/badge/node.js-%3E=_4.0.0-green.svg?style=flat-square
[node-url]: http://nodejs.org/download/
[download-image]: https://img.shields.io/npm/dm/rc-time-picker.svg?style=flat-square
[download-url]: https://npmjs.org/package/rc-time-picker

example
--------

http://react-component.github.io/time-picker/

install
-------

```
npm install rc-time-picker
```

Usage
-----

```
import TimePicker from 'rc-time-picker';
import ReactDOM from 'react-dom';
ReactDOM.render(<TimePicker />, container);
```

API
---

### TimePicker

| Name                    | Type                              | Default                                       | Description                                                                                |
|-------------------------|-----------------------------------|-----------------------------------------------|--------------------------------------------------------------------------------------------|
| prefixCls               | String                            |                                               | prefixCls of this component                                                                |
| clearText               | String                            | 'clear'                                       |                                                                                            |
| disabled                | Boolean                           | false                                         | whether picker is disabled                                                                 |
| clearText               | String                            | clear                                         | clear text                                                                                 |
| open                    | Boolean                           | false                                         | current open state of picker. controlled prop                                              |
| defaultValue            | moment                            | null                                          | default initial value                                                                      |
| defaultOpenValue        | moment                            | moment()                                      | default open panel value, used to set utcOffset,locale if value/defaultValue absent        |
| value                   | moment                            | null                                          | current value                                                                              |
| placeholder             | String                            | ''                                            | time input's placeholder                                                                   |
| showHour                | Boolean                           | whether show hour                             |                                                                                            |
| showMinute                | Boolean                         | whether show minute                             |                                                                                            |
| showSecond              | Boolean                           | whether show second                           |                                                                                            |
| format                  | String                            |                                               |                                                                                            |
| disabledHours           | Function                          | disabled hour options                         |                                                                                            |
| disabledMinutes         | Function                          | disabled minute options                       |                                                                                            |
| disabledSeconds         | Function                          | disabled second options                       |                                                                                            |
| hideDisabledOptions     | Boolean                           | whether hide disabled options                 |                                                                                            |
| onChange                | Function                          | null                                          | called when select a different value                                                       |
| addon                   | Function                          | nothing                                       | called from timepicker panel to render some addon to its bottom, like an OK button. Receives panel instance as parameter, to be able to close it like `panel.close()`.|
| placement               | String                            | bottomLeft                                    | one of ['left','right','top','bottom', 'topLeft', 'topRight', 'bottomLeft', 'bottomRight'] |
| transitionName          | String                            | ''                                            |                                                                                            |


## Test Case

```
npm test
npm run chrome-test
```

## Coverage

```
npm run coverage
```

open coverage/ dir

License
-------

rc-time-picker is released under the MIT license.
