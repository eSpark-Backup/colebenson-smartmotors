# ColeBenson-SmartMotors
 To create a smart motor system involving CAN Interface using STM32 MCU

## Project Requirements v3.3
* The RJ11 connector for CAN should be changed with RJ45 connector. The recommended connectors and pinouts are shared by client as stated below. We need to ensure that user can plug into any of the CAN connectors (CANA or CANB) and still have daisy chain feature without hassle. We will be restricting the user to only use Straight Through cable. 
    * ### Pinout Information
      ![image](https://github.com/eSpark-Consultants/ColeBenson-SmartMotors/assets/76909080/5c47f234-a592-4b93-8c52-1508aaad58f8)

    * ### Recommended Connector
        * [Digikey Link](https://www.digikey.ca/en/products/detail/molex/0855115001/2421532); [Molex Link](https://www.molex.com/en-us/products/part-detail/855115001)

    * ### Question
      We need to check if we need to restrict the user to only connect from CANA to CANA or CANB to CANB or they can also connect from CANA to CANB in daisy chain?

* Remove all Solder bridges from the design from both Top Board and Bottom board. Following bridges were sent by Japan team but they need to be ensured.
    * [Top Board]  
      SB6  
      SB3  
      SB9  
      SB4  
      SB11  
      SB7  
      SB1  
    * [Bottom Board]  
      SB2  
      SB4  
      SB6  
      SB8

* Add another high current Stepper Motor connector to the design and add it overlapping the existing connector. The suggested connector is [Digikey Link](https://www.digikey.ca/en/products/detail/jst-sales-america-inc/B4P-VH-FB-B-LF-SN/7230471)
* Change boot mode to be able to use a single 1 x 3 header with the center pin always GND.
