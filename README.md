# C3C Engineering

C3C, a concrete block company, is on a mission to make their blocks smarter. They want to add sensors to their concrete blocks, turning them into smart blocks. By doing this, C3C aims to bring loads of benefits to their customers and make a positive impact on society. They're diving into the world of Internet of Things (IoT) and AI, exploring exciting possibilities and creating unique products. 

* [C3C Engineering](#c3c-engineering)
* [General IoT Applications](#general-iot-applications)
   * [Microclimate](#microclimate)
   * [Gases](#gases)
   * [Sound](#sound)
   * [Object detection](#object-detection)
* [Safety and Monitoring in Biomass Storage](#safety-and-monitoring-in-biomass-storage)
* [Outcome](#outcome)
   * [Short term: Hardware proposal](#short-term-hardware-proposal)
      * [Temperature](#temperature)
      * [Humidity](#humidity)
      * [Methane (CH4)](#methane-ch4)
      * [Central Unit](#central-unit)
      * [HW Setup](#hw-setup)
   * [Long term: Research project - Bio+](#long-term-research-project---bio)

# General IoT Applications 

By providing solutions with IoT-enabled functionalities, C3C can offer their customers the flexibility to upgrade their concrete blocks with advanced features, making their products more intelligent, efficient, and adaptable to various applications. Here are a few examples:

## Microclimate
C3C can develop smart sleeves or attachments that can be fixed/retrofitted onto the pre-manufactured concrete blocks. These smart sleeves can have embedded sensors to measure and monitor microclimate data such as temperature, humidity, and air pressure. By attaching these devices to the blocks, customers can easily gather accurate data about the microclimate conditions in specific areas where the concrete blocks are installed, such as outdoor spaces or construction sites. This data can help optimize maintenance efforts or aid in environmental monitoring.

## Gases 
Similarly, C3C can create add-on modules or attachments containing gas sensors that can be attached to the pre-manufactured concrete blocks. These modules can detect and measure various gases in the surrounding environment. This enables customers to monitor gas levels in specific locations, such as warehouses, industrial sites, or storage facilities. By offering these IoT-enabled gas sensing modules, C3C can help customers maintain a safe and healthy environment by alerting them to any potential gas leaks or hazardous conditions.

## Sound 
To measure sound levels, C3C can develop fixed/retrofitting solutions with integrated sound sensors that can be added to their existing concrete blocks. These sensors can capture and analyze audio data to monitor noise levels in different settings. Retrofitting the blocks with sound sensors allows customers to gather data on noise pollution levels in specific areas where the blocks are installed. This information can be valuable for urban planning, construction site management, or even for assessing the effectiveness of noise barriers in a given space.

## Object detection 
Regarding object detection, C3C can develop smart modules that can be integrated into the pre-manufactured concrete blocks. These modules can include sensors, cameras, or even computer vision technology to detect and track objects or movements in the vicinity. By retrofitting the blocks with these smart modules, C3C can offer enhanced security and safety features. For example, the blocks can be equipped with motion sensors to detect unauthorized access or movement in restricted areas. This provides an additional layer of security for construction sites, private properties, or other controlled environments.


# Safety and Monitoring in Biomass Storage
One of the use cases for C3C's concrete blocks is to build pockets for biomass storage. Storing biomass poses various risks such as fire hazards, toxic gas emissions, structural integrity risks, health hazards, and environmental impacts. To address these dangers, it is important to implement proper safety protocols and monitoring systems, including the integration of IoT technologies, which can effectively mitigate these risks. 


Biomass can, for example, catch fire due to a combination of factors, including chemical, biological, and physical processes that can lead to self-heating and spontaneous combustion. The primary factors that contribute to the ignition of biomass stored in piles, bales, or silos are moisture content, temperature, oxygen availability, and the presence of microorganisms. So reading these values can give a good indication of its current state. 

Biomass can also lose energy during storage due to several factors. One major contributor is the moisture content in biomass materials. The presence of moisture requires energy to evaporate, resulting in lower heating values and reduced energy efficiency. 

Moreover, the biological degradation of biomass can occur during storage, caused by microorganisms, fungi, or insects. This degradation process breaks down organic compounds, leading to energy loss. Monitoring humidity levels in biomass storage is crucial to prevent issues such as moisture-related decay, self-heating, or the growth of microorganisms. 

Additionally, inadequate storage conditions such as open piles or uncovered areas can cause heat loss through radiation, convection, and conduction. Biomass can also release volatile compounds during storage, which escape into the atmosphere, further reducing its energy content. 

Lastly, chemical reactions like oxidation can occur when biomass is exposed to oxygen, resulting in energy loss. To minimize energy loss during biomass storage, it is crucial to manage moisture content, maintain appropriate storage conditions, prevent exposure to oxygen and pests, and employ covered storage systems whenever possible. By implementing these measures, the energy efficiency and availability of biomass can be maximized.



# Outcome 

## Short term: Hardware proposal
Pragramtically, the first approach would be to start measuring the temperature, relative humidity, and methane levels in the biomass stacks. Due to time constraints, no prototype was actually assembled and tested at any site.

### Temperature

To monitor temperature in biomass storage, C3C can utilize [PT1000](https://www.energibutiken.se/en/pt1000-sensors/215-pt1000-high-temp-sensor-6x50mm-3-meter-02045.html) temperature sensors. These sensors can accurately measure the temperature of the biomass piles, bales, or silos. The PT1000 sensors can be integrated into the concrete blocks or attached as separate devices. One option is the PT1000 high-temperature sensor, which is suitable for measuring temperatures in the range of 0°C to +400°C. The PT1000 sensors can then be connected to a temperature converter, such as the [PT1000 to 0-10V transducer](https://www.energibutiken.se/en/measuring-transducers/235-matvardesomvandlare-pt1000-till-0-10-volt-06001.html), which provides a compatible output for the central unit to process and analyze the temperature data. The use of this sensor would require an additional device responsible for reading and transmitting the data. But 


### Humidity
C3C can use the [CHS-MSS](https://www.mouser.se/ProductDetail/TDK/CHS-MSS?qs=sGAEpiMZZMv1xWCHBjbGeekHTbfHXJe2RWHy44mjJ48%3D) humidity sensor for this purpose. The CHS-MSS sensor is capable of accurately measuring humidity levels and can be integrated into the concrete blocks or installed as separate devices. By monitoring humidity levels, C3C can identify potential moisture-related risks and take appropriate actions to maintain the optimal humidity range in biomass storage.



### Methane (CH4)

To detect and monitor methane gas levels, C3C can utilize methane sensors. Methane is a potential byproduct of biomass degradation, and its accumulation can lead to flammability and gas emission hazards. One option (of many) is the [E2618-CH4](https://www.evikon.eu/en/evikon-mci-m-1/methane-transmitter-e2618-ch4-p-439) methane transmitter, which is designed specifically for monitoring methane gas concentrations. The E2618-CH4 sensor can be integrated into the concrete blocks or installed separately. Another option is the [ES101-CH4](https://www.womaster.eu/products_detail_Smart-City-%EF%BC%86-Industrial-IoT_IoT-Environmental-%7C-Water-%7C-Parking-%7C-Waste-Bin-Sensors_ES101CH4.htm) sensor, which is suitable for monitoring methane concentrations in various applications. By continuously monitoring methane levels, C3C can detect any potential combustion risks or gas leaks in biomass storage.


### Central Unit

To collect and process data from the temperature, humidity, and methane sensors, a central unit (or several) will be needed. The type of sensors would affect the choice of unit. In this case, some sensors require 12V to operate, thus making devices such as the [ESP32 PLC 38AR](https://www.industrialshields.com/shop/034001000700-esp32-plc-38ar-2910?product=product.template%282910%2C%29#attr=1441,29,2241,2242,3728,2243,3805) a suitable choice. The ESP32 PLC 38AR is a logic controller (PLC) with a built-in Wi-Fi module. The ESP32 PLC 38AR can serve as the gateway to transmit sensor data to the cloud platform for further analysis. It can also provide real-time control capabilities, allowing for automated responses based on the data received from the sensors. To power the central unit and ensure reliable operation, a DIN rail power supply such as the [AC-DC, 120W, 1 Output 5A at 24Vdc](https://www.industrialshields.com/shop/is-ac24vdc5adin-din-rail-power-supply-ac-dc-120w-1-output-5a-at-24vdc-689?search=DIN+Rail+Powe-r+Supply&order=name+asc#attr=3648) can be used (with an off-grid system obviously).


### HW Setup
The following is how such a system would be assembled in practice. The off-grid system would supply power to the central unit through connecting blocks. Connecting blocks would be blocks with channels for wires to pass through on each side as illustrated in the figure below with the red dotted lines. 

| Module | Power | Pins |
| -------- | -------- | -------- |
| **(Temperature)** PT1000 TRANSDUCER to 0-10 volt     | 24V     | IX.12     |
| **(Humidity)** CHS-MSS                               | 5V      | IX.11     |
| **(Methane)** E2618-CH4                              | 24V     | RS485 Modbus RTU or 0-10V    |

### 
![Alt text](/images/image.png)

## Long term: Research project - Bio+

The unexpected yet promising outcome of this project is the initiation of a substantial project application for Energimyndigheten. This initiative is a collaborative effort involving reputed institutions such as the Swedish Agricultural University (SLU), Linnaeus University, Linköping University, RISE, C3C, and FLIR. Spearheaded by C3C and facilitated through their existing connections with SLU, this collaborative endeavor highlights the remarkable synergies achieved through industry-academia cooperation.

The prospective project holds immense potential for C3C, presenting them with an avenue to further their mission in a significant way. It is a vivid illustration of the tangible benefits of industry-academia partnerships, opening up a realm of opportunities that were previously unexplored. This collaboration not only bodes well for the growth and development of C3C as a company but also stands as a testament to the innovative spirit fostered through this project, potentially leading to groundbreaking developments in the field.
