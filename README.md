<img width="500" alt="image" src="https://github.com/user-attachments/assets/1bed6a22-8f47-4a25-8a15-9baef247d9f9"/> <img width="500" alt="image2" src="https://github.com/user-attachments/assets/52ac9067-f325-4bbf-b8aa-69f3547c585c"/>

This PCB integrates several sensors commonly found on a weather balloon and ties the I2C outputs of these sensors to an Adafruit Feather M0 Adalogger. Several additional ports are available, this PCB supports up to 6 I2C connections routed through the TCA9548A multiplexor, allowing multiple of the same sensor to be used. A 3-pin interface supplying 3V, GND and digital data input lines is included to interface with the MightyOhm geiger counter kit. The 3V line is supplied by using a buck converter to lower 5V to 3V. The size of the PCB is chosen so it can easily be attached to the geiger counter. As pictured below, the white PCB on top is attached to the geiger counter using standoffs.

![image](https://github.com/user-attachments/assets/71ee4a80-4b34-48bc-8c60-7c0f214ba419)

An OLED is included to report errors and display real-time data, shown in this photo:

![image](https://github.com/user-attachments/assets/453385d7-618b-4a67-822e-3d158a4a22c3)

A DS3231 RTC(real-time clock) is included to provide time stamps for data collected. A MPL3115A2 PT(pressure-temperature) sensor is mounted on the PCB for gauging altitude. When we launched the PCBs during the April 8th, 2024 eclipse; we added 2 more PT sensors and a UV sensor via the I2C terminal blocks connected to the MUX. 

Tools:
- Soldering iron, flux, solder

Bill of Materials:
- 1x [Adafruit Feather M0 Adalogger](https://www.adafruit.com/product/2796)
- 1x [MightyOhm Geiger Counter Kit++](https://mightyohm.com/blog/products/geiger-counter/)
- 1x [TCA9548A MUX](https://www.adafruit.com/product/2717)
- 1x [OLED Breakout Board](https://www.adafruit.com/product/684)
- 1x [DS3231 RTC](https://www.adafruit.com/product/3013)
- 1x [AMS1117 Buck Converter](https://www.amazon.com/Anmbest-AMS1117-3-3-4-75V-12V-Voltage-Regulator/dp/B07CP4P5XJ/ref=sr_1_3?crid=37L7UTJOVB3HT&dib=eyJ2IjoiMSJ9.dNdTz3xf0JlyTyIUX87bachtYZ4fJ1FvHqrDlyGFcNkDXdMzG32SLR0UKRBnglLci5d9JRzqS4mDMEeCkYQfhyZ24NFUszIYvXpYoe0QuZ0_N80pzL2Ez0E3Rtpr71TZbEfL6HJSWaaaLn0Ul5RQup8h1o5B3DxhqrPDVrzoPn4uLcjXBZnu_Z2C3pxzRcEFm30_iZ5W7-sf2zoPMJjYwXI-VbpCW5QQkhZkivVnMgU.hX62fo94EqSNTrBGZzGj5FG9tlrqV-c6Vn11pWWRGW4&dib_tag=se&keywords=3+pin+buck+converter&qid=1735335725&sprefix=3+pin+buck+convertor%2Caps%2C112&sr=8-3)
- 2x [MPL3115A2 PT Sensor](https://www.adafruit.com/product/1893)
- 1x [LTR390 UV Sensor](https://www.adafruit.com/product/4831)
- 1x [MB102 5V Power Supply](https://www.amazon.com/HiLetgo-Supply-Module-Prototype-Breadboard/dp/B00HJ6AE72/ref=sr_1_3?crid=2DKGUQ1Q716YF&dib=eyJ2IjoiMSJ9.Md0j3eGgkH5_jjNUeIM9MG7lovEA-jCHb_v28IreAFFRgz20i9V9T2PUOIprbcB9NPysT5CcuoYPreC1EBqVbeTAHV1EzLlvSE8d7lZOWMyAWDkLV5m8z4J7JlNRYkzn4P8lAvpFpIHOB0atov4bzzMPYq5mAwt2YM9V5_ZTV-evMcT8-pG_v6qdllvFZ8q5WexeRxJlvpkwYed41cO5lWJdZB8AZoLQ1N6sVNaTb14.gvRQ09DsexbLZmC-hcVswSj8bGLP5GAwjicZ1Q906Mc&dib_tag=se&keywords=5v+supply+breadboard&qid=1735335704&sprefix=5v+supply+breadborad%2Caps%2C121&sr=8-3)
- 80x [female-male header pins](https://www.amazon.com/Glarks-Straight-Connector-Assortment-Prototype/dp/B076GZXW3Z/ref=sr_1_11?crid=303NKPL61S3C5&dib=eyJ2IjoiMSJ9.tG0DHq-qOQb29Ii9gxxXhT1xr975eEtKwB6Im_jWpigu4KK1BwF6S3hdOCO_plB4wKW28YRv5pRvOPg27KarTVW9WKEd7u0q5qevB1gAOurtL_dC1HtGhh-E6zim05gLTvGyZWysP__IFLbx-UyTL9_WVs8ldQev39iACwtP14eEVMWE2_FTbho3Kr8kW_224-88diKcYMWfBZL0xFa11DcUSFNvVPUOnnFHCmn80zGBVDPc2UgtcyQnQSPvPBjcT7kzkHKVVyIcws3OzayHrCVwi4_UbBevYlzZ796I5LHinkKAJ-gIo8s2m9VBaTiNmsMnC6YYV4gMnd6y3AbDiJ145Trr7vOGophGdx_4iZA.5Jt16vUwbAf6AtzjjqUpi08kPeEmf0GAt4aiNKbT_Po&dib_tag=se&keywords=female+male+header+pins&qid=1735334746&s=industrial&sprefix=female+male+header+pins%2Cindustrial%2C111&sr=1-11)
- 6x [4P Screw Terminal Block](https://www.amazon.com/Connector-Minidodoca-Terminals-Cable%EF%BC%8CEquipped-Screwdriver/dp/B0D29QD1WB/ref=sr_1_3?crid=3KMM1ABOXPGA2&dib=eyJ2IjoiMSJ9.mYsdZzL6FGqmLxdBz8OHnkKHsODyPVATk6LN_mVjZR1Ci2QxcgeG6KFm8H_nUql5fEM5-Bvcm922PfHZsN2928UapDtYTOkzUcqYkmNe2wrvzWjJhs2IwERjaNx7-eFfEOn5ujXpNInhK9wWqX0kfR0PvxI4a_ZPa2qNRIKmKRDRGQEkh989Cdgz_hzs3pJSeka7UZedNBv_VtW2O9UQFsfUVZIPEQs_ljjS_03p4AFrdZnTnrUl4xApC9YpJP20SvI_mjifPgT2EYtZTthUX5PPLjj64O1oIFFeDHVF0UDi2b0_dAArTpnCHg9GD9WaxeyJslS1bOWVABWaFBBU_fS6_ZGAlmMRkWvfw2F9jBM.NS5-iuKOMLw5ewH-8pB3pjTPDAJahAFMUU-Gm2kogmY&dib_tag=se&keywords=5pcs+16-Pin+%2816+Pole%29+Plug-in+Screw+Terminal+Block+Connector+2.54mm+0.1%22+Pitch+Panel+PCB+Mount+DIY&qid=1735334311&s=industrial&sprefix=5pcs+16-pin+16+pole+plug-in+screw+terminal+block+connector+2.54mm+0.1+pitch+panel+pcb+mount+diy%2Cindustrial%2C149&sr=1-3) and 1x [3P Screw Terminal Block](https://www.amazon.com/Connector-Minidodoca-Terminals-Cable%EF%BC%8CEquipped-Screwdriver/dp/B0D29QD1WB/ref=sr_1_3?crid=3KMM1ABOXPGA2&dib=eyJ2IjoiMSJ9.mYsdZzL6FGqmLxdBz8OHnkKHsODyPVATk6LN_mVjZR1Ci2QxcgeG6KFm8H_nUql5fEM5-Bvcm922PfHZsN2928UapDtYTOkzUcqYkmNe2wrvzWjJhs2IwERjaNx7-eFfEOn5ujXpNInhK9wWqX0kfR0PvxI4a_ZPa2qNRIKmKRDRGQEkh989Cdgz_hzs3pJSeka7UZedNBv_VtW2O9UQFsfUVZIPEQs_ljjS_03p4AFrdZnTnrUl4xApC9YpJP20SvI_mjifPgT2EYtZTthUX5PPLjj64O1oIFFeDHVF0UDi2b0_dAArTpnCHg9GD9WaxeyJslS1bOWVABWaFBBU_fS6_ZGAlmMRkWvfw2F9jBM.NS5-iuKOMLw5ewH-8pB3pjTPDAJahAFMUU-Gm2kogmY&dib_tag=se&keywords=5pcs+16-Pin+%2816+Pole%29+Plug-in+Screw+Terminal+Block+Connector+2.54mm+0.1%22+Pitch+Panel+PCB+Mount+DIY&qid=1735334311&s=industrial&sprefix=5pcs+16-pin+16+pole+plug-in+screw+terminal+block+connector+2.54mm+0.1+pitch+panel+pcb+mount+diy%2Cindustrial%2C149&sr=1-3)



