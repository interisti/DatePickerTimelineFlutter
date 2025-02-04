# DatePickerTimeline

[![Pub](https://img.shields.io/pub/v/date_picker_timeline?color=%232bb6f6)](https://pub.dev/packages/date_picker_timeline)

Flutter Date Picker Library that provides a calendar as a horizontal timeline.

<p>
 <img src="https://raw.githubusercontent.com/iamvivekkaushik/DatePickerTimelineFlutter/master/screenshots/demo.gif?raw=true"/>
</p>

## How To Use

Import the following package in your dart file

```
import 'package:date_picker_timeline/date_picker_timeline.dart';
```

## Usage

Use the `DatePickerTimeline` Widget

```
    Column(
        mainAxisAlignment: MainAxisAlignment.center,
        children: <Widget>[
          DatePickerTimeline(
            DateTime.now(),
            onDateChange: (date) {
              // New date selected
              print(date.day.toString());
            },
          ),
        ],
    ),
```

##### Constructor:

```
    DatePickerTimeline(
        this.currentDate, {
        Key key,
        this.dateSize = Dimen.dateTextSize,
        this.daySize = Dimen.dayTextSize,
        this.monthSize = Dimen.monthTextSize,
        this.dateColor = AppColors.defaultDateColor,
        this.monthColor = AppColors.defaultMonthColor,
        this.dayColor = AppColors.defaultDayColor,
        this.selectionColor = AppColors.defaultSelectionColor,
        this.onDateChange,
      }) : super(key: key);
```

Author
------

* [Vivek Kaushik](http://github.com/iamvivekkaushik/)


Contributors
------------
* [BradInTheUSA](https://github.com/bradintheusa)
