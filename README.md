# C3C Engineering

C3C, a concrete block company, is on a mission to make their blocks smarter. They want to add sensors to their concrete blocks, turning them into super cool smart blocks. By doing this, C3C aims to bring loads of benefits to their customers and make a positive impact on society. They're diving into the world of Internet of Things (IoT) and AI, exploring exciting possibilities and creating unique products. Get ready for a concrete revolution!

# General IoT Applications 

# Biomas condition monitoring

## Bill of Material

### Temperature
- [PT1000 temperature sensor](https://www.energibutiken.se/en/pt1000-sensors/215-pt1000-high-temp-sensor-6x50mm-3-meter-02045.html)
- [PT1000 TRANSDUCER to 0-10 volt
](https://www.energibutiken.se/en/measuring-transducers/235-matvardesomvandlare-pt1000-till-0-10-volt-06001.html)
- *[K120RTD - Temperature Converter Pt100](https://www.elfa.se/en/temperature-converter-pt100-ni100-200-650-seneca-k120rtd/p/30074420?ext_cid=shgooaqsesv-Shopping-PerformanceMax-CSS&&cq_src=google_ads&cq_cmp=18208288444&cq_con=&cq_term=&cq_med=pla&cq_plac=&cq_net=x&cq_pos=&cq_plt=gp&gclid=Cj0KCQjwnrmlBhDHARIsADJ5b_ldCyYDTifrTHSV_9PPrfXAJcUq57Rhh7RKIH8GwOLTIgl0vjd82d0aAug0EALw_wcB&gclsrc=aw.ds)

### Humidity
- [CHS-MSS](https://www.mouser.se/ProductDetail/TDK/CHS-MSS?qs=sGAEpiMZZMv1xWCHBjbGeekHTbfHXJe2RWHy44mjJ48%3D)

### Methane (CH4)
- [E2618-CH4](https://www.evikon.eu/en/evikon-mci-m-1/methane-transmitter-e2618-ch4-p-439)
- *[ES101-CH4](https://www.womaster.eu/products_detail_Smart-City-%EF%BC%86-Industrial-IoT_IoT-Environmental-%7C-Water-%7C-Parking-%7C-Waste-Bin-Sensors_ES101CH4.htm)

### Central Unit
- [ESP32 PLC 38AR](https://www.industrialshields.com/shop/034001000700-esp32-plc-38ar-2910?product=product.template%282910%2C%29#attr=1441,29,2241,2242,3728,2243,3805)
- [DIN RAIL Power Supply, ac-dc, 120W, 1 Output 5A at 24Vdc](https://www.industrialshields.com/shop/is-ac24vdc5adin-din-rail-power-supply-ac-dc-120w-1-output-5a-at-24vdc-689?search=DIN+Rail+Power+Supply&order=name+asc#attr=3648)


### HW Setup

| Module | Power | Pins |
| -------- | -------- | -------- |
| **(Temperature)** PT1000 TRANSDUCER to 0-10 volt     | 24V     | IX.12     |
| **(Humidity)** CHS-MSS                               | 5V      | IX.11     |
| **(Methane)** E2618-CH4                              | 24V     | RS485 Modbus RTU and 0-10V    |
