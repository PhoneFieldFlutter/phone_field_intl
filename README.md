# Flutter Phone Field Package

[![pub package](https://img.shields.io/pub/v/intl_phone_field.svg)](https://pub.dev/packages/intl_phone_field)
[![CI](https://github.com/vanshg395/intl_phone_field/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/vanshg395/intl_phone_field/actions/workflows/ci.yml)

A simple Flutter TextFormField to input an international phone number along with a country code.

This widget creates a text field to take a phone number input for any country along with an option to choose a country code.

## Screenshots

<img src="https://github.com/vanshg395/intl_phone_field/blob/master/1.png?raw=true" height="500px"> <img src="https://github.com/vanshg395/intl_phone_field/blob/master/2.png?raw=true" height="500px"> <img src="https://github.com/vanshg395/intl_phone_field/blob/master/3.png?raw=true" height="500px">

## Installing

To use the latest version of this package, add a dependency to your project using `git` syntax:

```yaml
dependencies:
  flutter_intl_phone_field:
    git:
      url: git://github.com/FlutterPhoneNumberField/flutter_intl_phone_field.git
      ref: master
```

## How to Use

Simply create a `IntlPhoneField` widget, and pass the required params:

```dart
IntlPhoneField(
    decoration: InputDecoration(
        labelText: 'Phone Number',
        border: OutlineInputBorder(
            borderSide: BorderSide(),
        ),
    ),
    initialCountryCode: 'IN',
    onChanged: (phone) {
        print(phone.completeNumber);
    },
)
```

Use `initialCountryCode` to set an initial Country Code.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Original Creators

- [Vansh Goel](https://github.com/vanshg395/)
- [Alex N'Guessan](https://github.com/marcaureln/)


