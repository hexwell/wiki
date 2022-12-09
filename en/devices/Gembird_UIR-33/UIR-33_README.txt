There are three drivers for the Gembird UIR-33 USB to IrDA adapter:

- one for the USB controller (ONE USB Compound Serial Device) (OneUComp.inf)
- one for the serial port (USB-to-One-Serial Port) (OneUPort.inf)
- a generic serial port to IrDA driver (netirsir.inf)

Of the first two, specific to the Gembird UIR-33 device, only unsigned versions were found (in UIR-33_driver[...].zip).
The third one is a generic driver used by many devices, including Irdroid USB to IrDA adapter.
Fortunately the latter has a signed version of this driver (Irdroid_irDA_Driver.zip).
