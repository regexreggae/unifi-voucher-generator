# UniFi Voucher Generator

Generates UniFi Hotspot vouchers using the UniFi controller API ready for printing. Customise the design using CSS.

This should work on any Linux/Mac machine that can reach the UniFi controller.

**Feb 2020**: Now works with UniFi 5.12.35 Controller.

![Preview of generated output](preview.png)

## Setup

1. Clone the repo:

```
git clone https://github.com/davidmaitland/unifi-voucher-generator.git
```

2. Set the variables in `unifi-api.sh` with your controller's details (username, password, baseurl, site).

3. Optionally customise the variables in `gen.sh` and the styles in `style.css`.

## Run

1. Run `./gen.sh` $time $amount $note // for example: ./gen.sh 60 10 "sample comment"  -> generates 10 vouchers with a validity of 1h with "sample comment" as name / comment. 

Note: simply running `./gen.sh` without parameters will make use of default values for amount, time and comment that are specified in the script.

2. Open `vouchers.html` and print!
