# React Date Picker
This fork was created so that we could include `excludedDays` - which lets us make certain days of the week non-selectable. For example, we only do Costco deliveries on Monday, so we exclude all days except mondays for Costco.

## Configuration

- Change date format by passing a different date format in the props: `dateFormat: "YYYY/MM/DD"`
- Add placeholder text: `placeholderText: 'Click to select a date'` (Defaults to the selected date when no placeholder text is added)
- Give users a predefined date range: `minDate: moment()` & `maxDate: moment().add(5, 'days')` (this gives users the ability to select a date between today and 5 days in the future)
- Exclude a set of dates from those that are selectable: `excludeDates: [ moment(), moment('2015-01-01') ]` (prevent users from selecting today or Jan 1st, 2015)
- Set custom moment.js instance (could have defined custom locale settings): `moment: require('./foo/moment')`
- Set custom locale settings for locale: `locale: "cs"`
- Set date format for callendar: `dateFormatCalendar: "YYYY/MM/DD"`
- Set custom weekdays (for locale days): `weekdays: ['Ne', 'Po', 'Út', 'St', 'Čt', 'Pá', 'So']`

## License

Copyright (c) 2014 HackerOne Inc. and individual contributors. Licensed under MIT license, see [LICENSE](LICENSE) for the full license.
