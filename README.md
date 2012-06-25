# Sencha Touch 2 Slider Field Extended

This is an extended version of the Sencha Touch 2 Slider field with added helper input item.

# Features

- Dynamically changing input item beside the standard Sencha Touch 2 slider.
- Slider position changes based on the value of the input item and changes are reflected immidiately. 
- Position of the input helper can be set as config
- Accessible in code using `xtype`

# Example Usage

      {
        xtype: 'sliderfieldinput',
        name: 'slider_decimal',
        labelText: 'Decimal',
        label: 'Decimal',
        value: 3,
        minValue: 0,
        maxValue: 100,
        increment: 0.25
      }

## Using a custom valueMapper

      {
        xtype: 'sliderfieldtext',
        name: 'slider_decimal',
        labelText: 'Decimal',
        label: 'Decimal',
        value: 0,
        minValue: 0,
        maxValue: 2,
        increment: 1,
        valueMapper: function(value) {
          self.config.valueMap[value];
        },
        valueMap: ['A', 'B', 'C']
      }

## Using auto-values

This will use values matching the valueMap passed in, in this example from 0 to 2, with initial value of 0 (override using defaultValue).

      {
        xtype: 'sliderfieldtext',
        name: 'slider_decimal',
        labelText: 'Decimal',
        label: 'Decimal',
        autoValues: true,
        valueMap: ['Any', 'Apartment', 'House']
      }


# Screenshots

![ios-screenshot](https://raw.github.com/nettantra/Sencha-Touch-2-SliderExtended/master/Screenshots/iOS-Screenshot.png)

![android-screenshot](https://raw.github.com/nettantra/Sencha-Touch-2-SliderExtended/master/Screenshots/Android-Screenshot.png)

