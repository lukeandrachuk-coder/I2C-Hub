The purpose of this project is to make a board that expands the number of I2C connective devices that you can connect to a microcontroller. The board was designed in KiCAD a free PCB design software. How it works is you connect the VCC, GND, SCL, and SDA from your microcontroller to the same ports in the I2C_In pins on the I2C hub board. You can then connect one or more of the eight out pins to your I2C devices.

<img width="602" height="418" alt="image" src="https://github.com/user-attachments/assets/3e37bec6-6fe9-4e05-bba2-6283e08d913f" />
<img width="512" height="316" alt="image" src="https://github.com/user-attachments/assets/a11e865a-8055-4d76-9fc2-2508de6206b1" />

# Assembly instructions: 
  First the TCA9546APWR chip needs to be soldered to the board. I recommend using solder paste for this as it is a surface-mount device. 
  
<img width="527" height="349" alt="I2C board 1" src="https://github.com/user-attachments/assets/22354a8e-e1ae-48ce-b620-8fe84b8d0d07" />

  Next solder the corresponding resistors in their places as well as the ceramic capacitor and LED. Lastly, solder the male pin headers into their spots. You should have nine 4-pin headers, and three 3-pin headers. 
  
<img width="527" height="349" alt="Screenshot 2026-10-20 123908" src="https://github.com/user-attachments/assets/587fc93e-aa19-44ab-978f-977459518951" />

  The 3-pin headers allow you to change the I2C address of the board based on which endpin you connect to the centre. One will pull it low (0), and the other will pull it high (1), letting you very the I2C address so it does not get confused with other I2C boards in code.
  
<img width="113" height="110" alt="Screenshot1 2026-10-20 123908" src="https://github.com/user-attachments/assets/81a63b55-6790-4ae1-95e7-8a50825e7d4e" />

# BOM

You must order the PCB from JLCPCB*, the link I have provided takes you to the online PCB quote page. You must upload the provided greber files .zip then select the PCB colour you want (any colour exept green takes longer to ship). You can leave all the other options alone.
<table>
  <thead>
    <tr>
      <th style="border: 1px solid #dddddd; padding: 8px; text-align: left;">Item</th>
      <th style="border: 1px solid #dddddd; padding: 8px; text-align: left;">Qty</th>
      <th style="border: 1px solid #dddddd; padding: 8px; text-align: left;">Supplier</th>
      <th style="border: 1px solid #dddddd; padding: 8px; text-align: left;">Cost/item</th>
      <th style="border: 1px solid #dddddd; padding: 8px; text-align: left;">Total Cost</th>
      <th style="border: 1px solid #dddddd; padding: 8px; text-align: left;">link</th>
    </tr>
  <thead>
  <tbody>
     <tr>
      <td style="border: 1px solid #dddddd; padding: 8px;">I2C Hub PCB</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">5</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">JLCPCB</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">N/A</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">$5.61</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">https://cart.jlcpcb.com/quote?from=pcbassembly_page</td>
    </tr>
    <tr>
      <td style="border: 1px solid #dddddd; padding: 8px;">TCA9546APWR</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">5</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Digikey</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">$2.12</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">$10.60</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">https://www.digikey.ca/en/products/detail/texas-instruments/TCA9546APWR/4842201</td>
    </tr>
     <tr>
      <td style="border: 1px solid #dddddd; padding: 8px;">2.54mm male pin headers</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">1</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Amazon</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">$3.59</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">$3.59</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">https://www.amazon.ca/2-54mm-Single-Socket-Breakaway-Connectors/dp/B0H9M69F4F/ref=sr_1_28?dib=eyJ2IjoiMSJ9.yTvO4Ctxl0OUyRyW3pki7Tqhjb_15nBXmuAJZeGEDNMo0eCxgBYOPyxYXSXgiYb4ljKhB2EOc_AQCAfljvOxCJ1Xxm2OkeHzCJ0IBh2KbvS-aUOyQDNqCzc6Uboud4w_PwxPd1CnfKyz1QM7oZLSZMhPvx28IleQ-zvfp2LupoBJt2vVJot_V8wWuBBqPMD4x6SXMQZKH2Puiv3ejK01JE38yJ67acV-_RkHXEawoAUQtakQwPXnNQur8iJZCgJsKgFyXAcIHZpj9kGQyyEAC8b53asezkW5_Me8TBcmNrY.DG0-hsSwsN1YIFz_b5xScE9tyFhYPBRk2B2CW9RvPzQ&dib_tag=se&gad_source=1&hvadid=788542685418&hvdev=c&hvexpln=0&hvlocphy=9189569&hvnetw=g&hvocijid=1598390221780357774--&hvqmt=b&hvrand=1598390221780357774&hvtargid=kwd-2493940636015&hydadcr=28046_14944998&keywords=2.54+mm+male+header+pins&mcid=5f4d9b8a47033eab997e191b3ade675b&qid=1791668972&refinements=p_36%3A-1000&rnid=12035759011&sr=8-28</td>
    </tr>
    <tr>
      <td style="border: 1px solid #dddddd; padding: 8px;">K104K15X7RF5TL2</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">5</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Digikey</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">$0.43</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">$2.15</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">https://www.digikey.ca/en/products/detail/vishay-beyschlag-draloric-bc-components/K104K15X7RF5TL2/286538</td>
    </tr>
      <tr>
      <td style="border: 1px solid #dddddd; padding: 8px;">CF14JT4K70</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">10</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">Digikey</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">$0.04</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">$0.40</td>
      <td style="border: 1px solid #dddddd; padding: 8px;">https://www.digikey.ca/en/products/detail/stackpole-electronics-inc/CF14JT4K70/1741428</td>
    </tr>
  </tbody>
<table>

  Plus tax and shipping.

  *I have chosen JLCPCB but you can use any manufacturer you want.
