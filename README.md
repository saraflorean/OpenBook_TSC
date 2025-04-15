# OpenBook_TSC

## Florean Sara-Denisa - 333CD

# Diagrama Block

<img width="1724" alt="Diagrama Block" src="https://github.com/user-attachments/assets/60ed80fb-ecaf-488f-957a-cd178b3270a1" />

---

# Descrierea modulelor hardware

## Microcontroler – ESP32-C6-WROOM-1-N8

ESP32-C6 este unitatea centrală de procesare responsabilă pentru gestionarea tuturor operațiunilor sistemului, comunicarea cu senzorii și modulele, precum și managementul energiei.

- **Arhitectură:** RISC-V pe 32 de biți  
- **Frecvență ceas:** 160 MHz  
- **Conectivitate wireless:** Wi-Fi 6 la 2.4 GHz, Bluetooth 5.0  

## Management Energetic & Baterie

- **Tip baterie:** Li-Po (Litiu-Polimer)  
- **Capacitate:** 3.7V, 1800mAh  
- **Circuit de încărcare:** MCP73831T  
- **Tensiune de intrare:** 5V prin USB-C  
- **Protecții:** Protecție la supraîncărcare și descărcare profundă  
- **Regulator de tensiune:** Regulator LDO care asigură o alimentare stabilă de 3.3V pentru toate componentele
  
## Afișaj – Ecran E-Paper (E-Ink)

- **Dimensiune:** 7.5 inci  
- **Rezoluție:** 800x480 pixeli  
- **Interfață de comunicare:** SPI  

## Modul Card SD

- **Tip:** MicroSD (Suportă FAT32)  
- **Interfață:** SPI  

## Memorie NOR Flash Externă

- **Capacitate:** 64MB  
- **Interfață:** SPI  

## Senzor de Mediu – BME688

- **Funcții:** Măsoară temperatura, umiditatea, presiunea aerului și nivelurile de gaz  
- **Interfață de comunicare:** I2C  

## Ceas în Timp Real (RTC) – DS3231SN

- **Funcționalitate:** Păstrează ora și data chiar și atunci când sistemul este oprit  
- **Interfață de comunicare:** I2C  

## Conector USB-C & Protecție ESD

- **Funcționalitate:** Asigură alimentarea și transferul de date  
- **Protecție:** Protecție ESD integrată și diodă Schottky pentru protecție la polaritate inversă  

## Butoane & Interacțiune cu Utilizatorul

- **Butoane tactile (push):** Utilizate pentru control manual  

## Interfețe de Comunicație

- **GPIO:** Folosit pentru controlul butoanelor și operațiuni generale I/O  
- **SPI:** Utilizat pentru cardul SD, memoria flash externă și ecranul e-paper  
- **I2C:** Utilizat pentru senzorul de mediu BME688 și modulul RTC DS3231SN  
- **UART:** Utilizat pentru depanare și comunicație serială  
- **Wi-Fi & Bluetooth:** Asigurate de ESP32-C6 pentru conectivitate wireless  

---

## Lista Componentelor folosite

| Componentă | Link | Fișă Tehnică |
|-----------|--------------|-----------|
| MAX17048G+T10 | [Model](https://www.snapeda.com/parts/MAX17048G+T10/Analog+Devices/view-part/?ref=eda) | [Datasheet](https://www.alldatasheet.com/view.jsp?Searchword=Max17048&gad_source=1&gbraid=0AAAAADcdDU8aYfZtfJfdZ9I5j6RwZ_cbA&gclid=Cj0KCQjwqcO_BhDaARIsACz62vNa9xrVfzjCjADRwXD0RBbo4Nret3ywwteDGLJKZui8ZL8KdVlTE7caAvQxEALw_wcB) |
| MCP73831T-5ACI/OT | [Model](https://www.mouser.co.uk/ProductDetail/Microchip-Technology/MCP73831T-5ACI-OT?qs=hH%252BOa0VZEiAcgAcEkuamXg%3D%3D) | [Datasheet](//efaidnbmnnnibpcajpcglclefindmkaj/https://ww1.microchip.com/downloads/en/DeviceDoc/MCP73831-Family-Data-Sheet-DS20001984H.pdf) |
| USB4110-GF-A  | [Model](https://componentsearchengine.com/part-view/USB4110-GF-A/GCT%20(GLOBAL%20CONNECTOR%20TECHNOLOGY)) | [Datasheet](//efaidnbmnnnibpcajpcglclefindmkaj/https://gct.co/files/drawings/usb4110.pdf) |
| Adafruit | [Model](https://eu.mouser.com/ProductDetail/Adafruit/4208?qs=PzGy0jfpSMtbScLbr0L5dw%3D%3D) | [Datasheet](https://www.arrow.com/en/manufacturers/adafruit-industries/datasheets) |
| CAPACITOR | [Model](https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO) | [Datasheet](//efaidnbmnnnibpcajpcglclefindmkaj/https://www.resistor.com/assets/pdf/0402tstd.pdf) |
| CPH3225A | [Model](https://www.snapeda.com/parts/CPH3225A/Seiko+Instruments/view-part/?ref=eda) | [Datasheet](https://octopart.com/datasheet/cph3225a-seiko-25340571) |
| EVQPUJ02K | [Model](https://industry.panasonic.com/global/en/products/control/switch/light-touch/number/evqpuj02k) | [Datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2201121800_PANASONIC-EVQPUJ02K_C2936858.pdf) |
| KP-1608SURCK | [Model](https://www.snapeda.com/parts/KP-1608SURCK/Kingbright/view-part/?ref=search&t=LED%200603) | [Datasheet](//efaidnbmnnnibpcajpcglclefindmkaj/https://media.elv.com/file/107153_led_surck1608_data.pdf) |
| USBLC6-2SC6Y | [Model](https://www.snapeda.com/parts/USBLC6-2SC6Y/STMicroelectronics/view-part/?ref=eda) | [Datasheet](https://www.digikey.com/en/htmldatasheets/production/1375342/0/0/1/usblc6-2sc6y) |
| SD0805S020S1R0 | [Model](https://ro.mouser.com/ProductDetail/KYOCERA-AVX/SD0805S020S1R0?qs=jCA%252BPfw4LHbpkAoSnwrdjw%3D%3D) | [Datasheet](https://www.alldatasheet.com/view.jsp?Searchword=SD0805S&sField=2) |
| PGB1010603MR | [Model](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) | [Datasheet](https://www.alldatasheet.com/view.jsp?Searchword=Pgb1010603mr&gad_source=1&gbraid=0AAAAADcdDU8aYfZtfJfdZ9I5j6RwZ_cbA&gclid=Cj0KCQjwqcO_BhDaARIsACz62vOPBOBe0eOh5gDUFkkKl4JBcbmoFZYtJ8BOnbaWqr_BuUCcVWvbutAaAmGkEALw_wcB) |
| BD5229G-TR  | [Model](https://componentsearchengine.com/part-view/BD5229G-TR/ROHM%20Semiconductor) | [Datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2201131330_ROHM-Semicon-BD5229G-TR_C962636.pdf) |
| BME680 | [Model](https://www.snapeda.com/parts/BME680/Bosch/view-part/?welcome=home) | [Datasheet](//efaidnbmnnnibpcajpcglclefindmkaj/https://www.bosch-sensortec.com/media/boschsensortec/downloads/datasheets/bst-bme680-ds001.pdf) |
| XC6220A331MR-G | [Model](https://componentsearchengine.com/part-view/XC6220A331MR-G/Torex) | [Datasheet](https://www.alldatasheet.com/view.jsp?Searchword=Xc6220&gad_source=1&gbraid=0AAAAADcdDU8aYfZtfJfdZ9I5j6RwZ_cbA&gclid=Cj0KCQjwqcO_BhDaARIsACz62vPS06NB6tLgniZzfaVpKNu1m811BNk6AEPfg4DbP6f5S8QWA_pW_UQaAv-0EALw_wcB) |
| SMD Solder | [Model](https://grabcad.com/library/solder-jumpers-1) | [Datasheet]() |
| BUTTON | [Model](https://industry.panasonic.com/global/en/products/control/switch/light-touch/number/evqpuj02k) | [Datasheet](https://www.lcsc.com/datasheet/lcsc_datasheet_2201121800_PANASONIC-EVQPUJ02K_C2936858.pdf) |
| Bobina | [Model](https://store.comet.srl.ro/Catalogue/Product/43497/) | [Datasheet](https://www.scribd.com/document/814581278/Datasheet-Bobina) |
| PFMF | [Model](https://www.mouser.co.uk/ProductDetail/EPCOS-TDK/B72520T0350K062?qs=dEfas%2FXlABIszF52uu7vrg%3D%3D) | [Datasheet](https://ro.mouser.com/c/ds/circuit-protection/thermistors/resettable-fuses-pptc/?m=Schurter&series=PFMF) |
| DMG2305UX-7 | [Model](https://componentsearchengine.com/part-view/DMG2305UX-7/Diodes%20Incorporated) | [Datasheet](//efaidnbmnnnibpcajpcglclefindmkaj/https://www.mouser.com/datasheet/2/115/DMG2305UX-266242.pdf?srsltid=AfmBOop22k34YTJJra1xubiU6LPiN4M4JlcWbRoSNdxSGFak8uWgXPpK) |
| Si1308EDL-T1-GE3 | [Model](https://componentsearchengine.com/part-view/SI1308EDL-T1-GE3/Vishay) | [Datasheet](https://www.alldatasheet.com/view.jsp?Searchword=Si1308edl&gad_source=1&gbraid=0AAAAADcdDU-px713ONYSnQ2O-gcwqYcFq&gclid=Cj0KCQjwqcO_BhDaARIsACz62vN_Nz3MJOc6J_03gnVBm7aSqC8v9wyP0VD-iRKP-gFrYgdhLi99I14aAlVJEALw_wcB) |
| R0402 | [Model](https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO) | [Datasheet](//efaidnbmnnnibpcajpcglclefindmkaj/https://www.resistor.com/assets/pdf/0402tstd.pdf) |
| W25Q512JVEIQ | [Model](https://www.snapeda.com/parts/ESP32-C6-WROOM-1-N8/Espressif+Systems/view-part/?ref=eda) | [Datasheet](//efaidnbmnnnibpcajpcglclefindmkaj/https://www.mouser.com/datasheet/2/949/W25Q512JV_SPI_RevB_06252019_KMS-2487502.pdf?srsltid=AfmBOoquExqDVgxEELF9CzuOGxHos0CD1nQDROHD6Eebdm2foNzqozqU) |
| ESP32-C6-WROOM-1-N8 | [Model](https://www.snapeda.com/parts/ESP32-C6-WROOM-1-N8/Espressif+Systems/view-part/?ref=eda) | [Datasheet](//efaidnbmnnnibpcajpcglclefindmkaj/https://www.mouser.com/catalog/specsheets/Espressif_ESP32_C6_WROOM_1%20_Datasheet_V0.1_PRELIMINARY_en.pdf?srsltid=AfmBOooHQKNitqODRaaPjoZInfWKTacDER1t5uRK6sKqT13TrzvVo_B7) |
| DS3231SN# | [Model](https://www.snapeda.com/parts/DS3231SN%23/Analog+Devices/view-part/?ref=eda) | [Datasheet](https://www.alldatasheet.com/view.jsp?Searchword=Ds3231sn%20datasheet&gad_source=1&gbraid=0AAAAADcdDU-Gy9URfMxGmqiPg7ci5L3wR&gclid=Cj0KCQjwqcO_BhDaARIsACz62vMkK3ETSnW2w7mo0Fa-wgWJGn89AxWCyIND6k5X8MmoPl6hv6VWwT8aAiS-EALw_wcB) |

---

## Mapare Pini – ESP32-C6

| Denumire       | Pin GPIO      | Utilizare                                |
|----------------|---------------|------------------------------------------|
| Buton Reset    | EN            | Resetare ESP32-C6                        |
| INT_RTC        | IO0           | Semnal de întrerupere de la RTC (DS3231)|
| 32KHZ          | IO1           | Semnal de ceas 32 kHz                    |
| MISO (SPI)     | IO2           | Recepție date SPI                        |
| EPD BUSY       | IO3           | Indicator stare E-Paper                  |
| SS_SD          | IO4           | Chip Select pentru card SD (SPI)        |
| EPD DC         | IO5           | Data/Command pentru E-Paper             |
| SCK (SPI)      | IO6           | Clock pentru SPI                         |
| MOSI (SPI)     | IO7           | Transmitere date SPI                     |
| Buton Boot     | IO9           | Intrare în bootloader                    |
| 3V3            | 3V3           | Alimentare 3.3V                          |
| EPD_CS         | IO10          | Selectare SPI pentru E-Paper            |
| FLASH_CS       | IO11          | Selectare SPI pentru NOR Flash          |
| USB_D-         | IO12          | Linie diferențială USB (minus)          |
| USB_D+         | IO13          | Linie diferențială USB (plus)           |
| Buton Change   | IO15          | Schimbare mod operare                    |
| TX (UART)      | TXD0/GPIO16   | Transmitere date UART                   |
| RX (UART)      | RXD0/GPIO17   | Recepție date UART                      |
| RTC_RST        | IO18          | Reset extern/semnal RTC                 |
| I2C_PW         | IO19          | Linie de alimentare / enable pentru I2C |
| EPD_3V3_C      | IO20          | Linie de alimentare 3.3V pentru E-Paper |
| SDA (I2C)      | IO21          | Linie de date I2C                       |
| SCL (I2C)      | IO22          | Linie de ceas I2C                       |
| EPD RST        | IO23          | Resetare E-Paper                        |

---

## Informații adiționale

**Erori SMD-Hole Board Outline Clearance la Mufa USB:**  
  - Am identificat două erori de tip **SMD-Hole Board Outline Clearance** asociate mufei USB. Conform informațiilor tehnice primite, aceste erori au fost **acceptate**.

**Redimensionarea și amplasarea componentelor:**
  - Dimensiunile unor componente au fost **ajustate** pentru a rezolva incompatibilitățile detectate de verificatorul de design.
  - Condensatori de decuplare de 100nF au fost **amplasați aproape de pinii de alimentare** ai circuitelor integrate (IC), în conformitate cu practicile standard de proiectare pentru reducerea zgomotului electric.
  - Componentele au fost amplasate respectând pe cât de mult posibil **specifcațiile proiectului** asigurând compatibilitatea dintre carcasa oferită și dimensiunile PCB-ului.
  - **TP-urile** au fost amplasate diferit față de specificațiile oferite, pentru a facilita o rutare eficientă. Poziția lor fiind determinată de apropierea de piesele conectate.

 **Rutare și planuri de masă**
 - **Traseele de alimentare** au fost rutate **doar pe stratul superior**, ceea ce a necesitat utilizarea a aproximativ 100 de vias-uri pentru a permite rutarea semnalelor pe stratul inferior.
 - **Planul de masă** (GND) a fost adăugat după finalizarea rutării, aplicat atât pe stratul superior, cât și pe cel inferior, pentru a asigura o împământare cu impedanță redusă și pentru a diminua interferențele electromagnetice (EMI).
 - Am realizat **via stitching** în regiunile unde planurile de masă de pe stratul superior și inferior se suprapuneau, pentru a asigura o conexiune electrică solidă între acestea.



