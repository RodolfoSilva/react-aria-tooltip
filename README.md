# react-aria-tooltip
Simple ReactJS component that adds the appropriate role, identification structure, and aria-hidden attribute for a tooltip.

## Installation
`npm install react-aria-tooltip`


## Usage
```
import ReactARIAToolTip from 'react-aria-tooltip'

return (
    <ReactARIAToolTip message="You custom message">
        <sometagorcomponent></sometagorcomponent>
    </ReactARIAToolTip>
)
```

You will also need to include the tooltip css path into your application in some form.

### CSS @import
Import the package css file relative to your `node_modules` directory.

Example
```
@import "../../../node_modules/react-aria-tooltip/dist/react-tooltip.min.css";
```

## Options
1. `message` string that will display in the tooltip
2. `eventType` this can either be 'click' or 'hover'
3. `direction` the placement of the tooltip. Can be one of four options 'top', 'bottom', 'right', 'left'
4. `duration` this is only applicable to the click `eventType`. This value defines the amount of time the tooltip is present after the user clicks the target element

## Examples
```
<ReactARIAToolTip message="Tooltip text" eventType="hover" direction="bottom">
    <span>Some text</span>
</ReactARIAToolTip>
```

```
<ReactARIAToolTip message="Something fancy" eventType="click" duration="500">
    <img src="../path/to/some/image" alt="" title="" />
</ReactARIAToolTip>
```

## MIT Licenced
