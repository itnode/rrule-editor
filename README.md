# <rrule-editor>

recurrence rules for calendar dates

## Install & Run

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) and [Bower](https://bower.io/#install-bower) installed. 

Then run following
```
bower install
polymer serve
```

Then run you can see demo app is serve at `http://127.0.0.1:8081/components/rrule-editor/demo/`

## How define the your Element

The element in slot is find by `data-` selector, Please make sure those are in `rrule-editor`
```
<rrule-editor>
    Event Date: <input data-id="date" type="date" name="begin" />
    Recurring:
    <select name="reccurend" data-id="date-reccurend">
        <option value="no">No</option>
        <option value="daily">Daily</option>
        <option value="weekly">Weekly</option>
        <option value="monthly">Monthly</option>
        <option value="yearly">Yearly</option>
        <option value="custom">Custom</option>
    </select>
    <input type="hidden" data-id="date-hidden"  name="rrule" value="" />
    <span data-id="date-reccurend-txt"></span>
</rrule-editor>
```

These 4 selector should be present in element `data-id="date"`, 
`data-id="date-reccurend"`, `data-id="date-hidden"`, `data-id="date-reccurend-txt"`
