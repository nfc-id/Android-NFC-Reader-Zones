# Android-NFC-Reader-Zones
This repository contains a JSON file with information about the NFC reader
position on various Android devices.

## Description

Many Android devices have their NFC reader located in different areas, which can
affect usability when scanning NFC tags. This JSON provides a list of devices
along with their NFC reader position, making it easier to integrate this
information into applications.

## JSON format

The JSON file follows this structure:

```
[
    {
        "manufacturer": "example",
        "deviceModel": "example",
        "deviceCommercialName": "example",
        "nfcReaderPosition": "top"
    }
]
```

Note that all fields content are in lower case.

### Possible positions

The `nfcReaderPosition` field can take one of the following values:
- `top`: reader located at the top of the device.
- `center` reader located at the center of the device.
- `bottom` reader located at the bottom of the device.
- `side` reader located on the side of the device. Applied only for one Xiaomi
device. See the _Xiaomi MIX Flip_ model in [Xiaomi NFC Areas](https://sf.pay.xiaomi.com/views/cmsModelPages/nfcArea.html).

## How to contribute

If you want to add more devices, you can make a pull request following these
rules:
- Maintain valid JSON format.
- Use official manufacturer and model names.
- Ensure the information is accurate.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more
details.
