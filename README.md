# DatePickerJS

A dependency-free (pure JS/CSS) date picker for Divi 5 Contact Form fields. Attach it by CSS ID; it formats dates as MM/DD/YYYY.

- `divi-date-picker.html` - paste-ready snippet (style + script + example calls). Paste into Divi > Theme Options > Integration > "Add code to the body", or into a Code Module.
- `demo.html` - local test page that mimics Divi markup (overflow:hidden parents, late-rendered field, scrolling container).

```js
attachDatePicker('#booking_date');
attachDatePicker('#service_date', { minDate: 'today', maxDate: '12/31/2027', disableWeekends: false });
```

Set the CSS ID on the Divi field (Advanced > CSS ID & Classes); the script finds the `<input>` inside the wrapper. Fields added after page load are picked up via MutationObserver.
