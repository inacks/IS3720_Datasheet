# IS3720_Datasheet
Datasheet of the IS3720 I2C DMX+RDM Receiver Integrated Circuit 

## What is it and what it does

The IS3720 is a chip that integrates both DMX Receiver + RDM Responder protocols in a single IC. It buffers all 512 DMX channels in its internal memory map, which is accessible by your microcontroller via I2C.

The IS3720 also enables bidirectional communications through RDM, allowing remote configuration and management of your product. This eliminates the need for manual setup, such as physically adjusting the DMX start address.

## Utility

RDM is especially helpful for light fixtures in large installations, such as building façade lighting, where an operator would otherwise spend significant time manually setting DIP switches on thousands of fixtures distributed across multiple floors and rooms.

It is also invaluable in installations where fixtures are embedded in the pavement or other sealed environments, like swimming pools or ornamental fountain where opening them would require breaking the ground or compromising waterproofing.

## Benefits

The IS3720 eliminates the need for engineers to learn and implement the low-level details of the DMX and RDM protocols. This significantly reduces development and testing effort, shortens time-to-market, and enables faster product release.

## How it works

The IS3720 features two communication interfaces:

- An I2C-serial interface (SCL and SDA pins), operating as slave device, used to communicate with your microcontroller.
- A UART interface (RX/TX and DIR pins), used for DMX+RDM communications using an RS485 transceiver.

The IS3720 has an internal memory map consisting of 632 registers. Registers 1 to 512 correspond directly to DMX channel values. For example, reading register address 1 gets the value of DMX Channel 1, reading register address 512 reads the value of DMX Channel 512, covering the full range of channels.

RDM registers are mapped after the DMX registers. Some are informational, such as the MANUFACTURER_LBL register block, where you write via I2C your company name and it will show up on the RDM controller. Others are operational, such as the DMX_START_ADDRESS register block, which indicates the assigned DMX start address.

## Buy

You can buy the product at:

- www.inacks.com/is3720

## Questions?

💬 Contact us anytime for support.

- www.inacks.com


## Others
- Tube packaging for pick-and-place available upon request.
- Volume-based pricing available upon request.

---

*This company and the products provided herein are developed independently and are not affiliated with, endorsed by, or associated with any official protocol or standardization entity. All trademarks, names, and references to specific protocols remain the property of their respective owners.*
