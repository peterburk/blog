# iPod Nano Flash Upgrade Fail
When software restricts hardware. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0839.jpg" target="_blank"><img class="aligncenter" alt="iPod Nano and TSOP48" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0839.jpg" width="128"></a>

## History
The iPod Nano 1G was the first flash-based iPod when it came out in September 2005. It came in three capacities: 1GB, 2GB, and 4GB. I liked the small physical size, but the capacity was just too small for my music library, which was over 20GB at the time. 

I was repairing iPods for friends at school and church, and I quickly looked for the iFixit teardown of the new iPod Nano. I was distraught. The battery and flash memory were soldered onto the motherboard! Upgrades seemed impossible. 

Fast forward 10 years. I went to university in the UK, graduated with a Masters degree in Electronic Systems Engineering, and moved to Taiwan to work for a flash memory manufacturer. I still use an iPod regularly (5.5G + iFlash-Dual + PQI Air Card), and friends here still ask me to fix their iPhones and iPods. Pastor Van from the KHOP prayer room asked me to upgrade his iPod Nano 1G battery, which had worn out over time. I realised that I now have access to the tools needed to upgrade the flash memory too! If I succeeded, I could create the first iPod Nano with more than 16GB capacity. The 16 year-old inside me was excited to finally see this happen!

## Plan
The iPod Nano 1GB and 2GB have blank spaces on their logic boards, while the 4GB iPod Nano has a second flash memory chip. What happens if I put a second flash memory chip into that space? 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0829.jpg" target="_blank"><img class="aligncenter" alt="iPod Nano and mSata SSD" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0829.jpg" width="128"></a>

## Getting a chip
The flash chip I need uses the TSOP48 package. I looked at photos online, and found out that iPod Nano uses chips from various manufacturers (Toshiba, Hynix, Samsung). I just needed to get any TSOP48. In November, I asked my boss about getting a chip from the factory, but decided in January to stop nagging and desolder one from another device. They’re pretty common in USB sticks and SD cards, but I can’t easily see if a device uses one. And I really want a chip that’s at least 16GB in capacity. 

Fail No. 1: Ordered a Kingspec iPod Video 128GB SSD, because it looks like it uses TSOP48 chips. When it arrived, I saw that it has BGA chips. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0898.jpg" target="_blank"><img class="aligncenter" alt="Kingspec" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0898.JPG" width="128"></a>

It doesn’t even work in my iPod Video 5.5G, which is a real disappointment. But it works as advertised in my iPod Video 5G, so I can’t return it. To Kingspec’s credit, it is super fast and low-power. But I did spend $100 on something I don’t need. 

Next, I hit the local electronics street. Kaohsiung’s got a decent selection of stores on Jianguo Road and Changming Street: fewer products but much more organised than Huaqiangbei in Shenzhen. Eventually I found out that a Kingston mSata 64GB SSD has the chip I need! That cost another $45. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0837.jpg" target="_blank"><img class="aligncenter" alt="TSOP48 from mSata SSD" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0837.jpg" width="128"></a>

## Desoldering
I first Superglued an ear-cleaner to the chip, melted the solder using a heat gun, and tried to pull the chip off the board. The glue melted. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0831.jpg" target="_blank">Glue</a>

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0832.jpg" target="_blank">Heat</a>

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0833.jpg" target="_blank">Fail</a>

Then I tried to hold the chip using tweezers. The grip wasn’t good enough to pull the chip. I figured out that holding the board off the workbench while heating would let gravity pull the board down when the solder melted. That worked!

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0836.jpg" target="_blank"><img class="aligncenter" alt="mSata SSD" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0836.jpg" width="128"></a>

Don’t forget to clean the connectors. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0850.jpg" target="_blank">Cleaning</a>

I also desoldered the battery from the iPod Nano. I really think that Apple should have used a connector here. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0838.jpg" target="_blank">Battery</a>

## Soldering
I thought that I’d get access to some fancy special tools. But my friend in the R&D lab couldn’t help me get into the factory, so I was stuck with standard workbench tools. 

The hardest part is to hold the chip in place. 
Tweezers don’t work. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0852.jpg" target="_blank">Tweezers</a>

A vice is hard to work with. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0856.jpg" target="_blank">Vice</a>

Eventually I used masking tape. After spending 20 minutes trying to aligning the chip, I asked my colleague Shu-Ting Yang to help. She’s much more talented! 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0857.jpg" target="_blank"><img class="aligncenter" alt="Masking tape" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0857.jpg" width="128"></a>

I took many photos to make sure that it was aligned correctly. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0858.jpg" target="_blank">Before heat</a>

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0859.jpg" target="_blank">Heating</a>

I managed to short out two pins on the original chip because the heat gun was too close. I cleaned that up with some more heat and a knife. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0860.jpg" target="_blank">Shorted</a>

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0869.jpg" target="_blank">Un-shorted</a>

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0871.jpg" target="_blank"><img class="aligncenter" alt="TSOP48 soldered" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0871.JPG" width="128"></a>

I know that the connections were strong because I pulled the tape off the chip, and it stayed on the logic board. 

Next, I soldered the battery back on and reassembled the iPod Nano. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0872.jpg" target="_blank">Battery</a>

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0873.jpg" target="_blank"><img class="aligncenter" alt="Shu-Ting Yang" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0873.jpg" width="128"></a>

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0874.jpg" target="_blank"><img class="aligncenter" alt="Peter Burkimsher" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0874.jpg" width="128"></a>

## Testing
The good news: it boots and connects to iTunes!

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0876.jpg" target="_blank">Booting</a>

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0877.jpg" target="_blank">Do Not Disconnect</a>

Diagnostics mode has a flash check, but doesn’t indicate the capacity. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0880.jpg" target="_blank">Diagnostics mode</a>

Fail No. 2: The iPod still thinks it’s only got 1GB capacity. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0878.jpg" target="_blank"><img class="aligncenter" alt="iTunes after mod" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_0878.JPG" width="128"></a>

## Conclusion
The mod didn’t work, but at least I didn’t break the iPod in the process. It was an expensive lesson. The 200GB iPod Nano on Uncyclopedia will remain a myth. 

<a href="http://uncyclopedia.wikia.com/wiki/Ipod_Nano_200gb_Instructions/Page_2#Step_4_-_Desoldering_Flash" target="_blank">Uncyclopedia</a>

I presume that it doesn’t work because the flash controller firmware is pre-programmed to only address 1GB of flash memory. This is technically a software problem. 

Lessons learned:
1. It’s faster to go to a shop than ask your boss for parts from the factory downstairs. 
2. Don’t trust pictures of products online. 
3. Just because there’s a connector doesn’t mean that you can just plug something into it. 

I still have my WiPod, though, so I’m satisfied for now. It’s the only iPod with WiFi, which works great to copy photos from SD cards to my iPhone. 

<a href="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_9640.jpg" target="_blank"><img class="aligncenter" alt="WiPod" src="https://raw.githubusercontent.com/peterburk/blog/master/ipodnanophotos/IMG_9640.JPG" width="128"></a>
