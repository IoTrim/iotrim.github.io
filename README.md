# IoTrim
Consumer IoT devices come with convenient services. However, since there are few strict privacy/security regulations and standards in the IoT context, device abuse is increasingly becoming a major privacy/security issue for consumers worldwide. 

IoTrim, automatically monitors and blocks non-essential network activities, and identifies IoT devices’ information exposure and security threats, using privacy-preserving AI techniques to build insights and behavioral models from devices.
IoTrim components run on the home router, and can be controlled through a smartphone app, a computer or the user’s voice (It offers easy-to-use, plug and play protection). 

IoTrim prevents violations of individuals’ privacy by intercepting and blocking information exposure to third-party analytics and service providers, most of which are collecting personal data unbeknownst to the user and potentially breaking privacy regulations such as the GDPR and CCPA.

The design of the testing system (<a href="https://github.com/IoTrim/IoTrigger">IoTrigger</a>), the blocking system (<a href="https://github.com/IoTrim/IoTrimmer">IoTrimmer</a>), the <a href="https://github.com/IoTrim/ML">AI Engine</a>, and the <a href="https://github.com/IoTrim/iotrimlist">IoTrim list</a> have now been released! 

## IoTrim List

This site contains a <a href="https://github.com/IoTrim/iotrimlist">set of non-required destinations list</a> from 31 consumer IoT devices and the software for producing the list. The list is created using a methodology for determining non-required destinations by automatically executing IoT device functions and determining the execution outcome while blocking selected destinations.
IoT devices offer multiple types of functionality; however, for this list, we select only the main functions for every IoT device under test. However, from preliminary experiments we have seen that most devices use the same destinations for different functions. 

<a href="https://github.com/IoTrim/iotrimlist/"><img src="https://raw.githubusercontent.com/IoTrim/iotrimlist/master/iotrim.png" width="500"/></a>

The list contains 4 columns: 

* device: the device under test
* destination: the non-required destination 
* party: destination’s party type (first party, third, support)
     - First party: destination related to the device manufacturer.
     - Support party: destination that is not a first party and is responsible for providing remote computation.
     - Third party: destination that is not a First party or a Support party. 
* grouped: to facilitate analysis and streamline blocklists, we developed a strategy to group destinations thet use different DNS names and IP addresses for each replica. 

## IoTrigger

This site contains a <a href="https://github.com/IoTrim/IoTrigger"> command-line version of IoTrigger</a>, which includes a library of probes and triggers scripts that support the IoT devices we tested. IoTrigger manages the lifecycle of functionality experiments for each device, including the invocation of user-provided trigger and probe scripts, and to finally produce (non-)required destination lists.
     
## IoTrimmer

This site contains a <a href="https://github.com/IoTrim/IoTrimmer"> version of IoTrimmer</a>. It comes preconfigured with the deny-listing blocking strategy and uses the blocklist of 62 non-required destinations we found for our set of 31 IoT devices. 
When a new device is connected to IoTrimmer its MAC address appears on the list.
The user then chooses which device is connected to IoTrimmer. The blocklist (IoTrim) is regularly updated from the Internet and automatically applied to all connected devices. Users can click on a device to display the list of blocked destinations.
     
## AI Engine

This site contains a <a href="https://github.com/IoTrim/ML"> version of the AI Engine</a>. The IoTrim AI Engine allows to build and re-train ML models for device identification.

## TEAM
IoTrim leverages advanced privacy preserving AI techniques for creating the trim lists. The protection techniques behind IoTrimmer have been reviewed by experts in top academic institutions, resulting in research papers published in top tier scientific conferences and EU/US funded research projects. Our team won important awards and our research has been featured in the Financial Times, New York Times, USA Today and the BBC. 

* <a href="https://annamandalari.com/">Dr Anna Maria Mandalari</a> works as Associate Professor at University College London (UCL). She is affiliated with the Electronic & Electrical Engineering Department and member of the UCL’s Academic Center of Excellence in Cyber Security Research (ACE-CSR).  She is Honorary Research Fellow at the Institute for Security Science and Technology at Imperial College London. Her research interests are related to IoT, privacy, large-scale Internet measurements, Internet measurement platforms, middleboxes and new Internet protocols. 

* <a href="https://haddadi.github.io/">Professor Hamed Haddadi</a> is an Associate Professor in Human-Centred Systems at the Department of Computing at Imperial College London. He is part of the Networks and Systems Laboratory (NetSys) and Imperial-X (I-X) where he leads the Privacy and Security Research Area. He also serves as a Security Science Fellow of the Institute for Security Science and Technology. In his industrial role, he is the Chief Scientist at Brave.

* <a href="https://david.choffnes.com/">Professor David Choffnes</a> is an Associate Professor at Northeastern University, Executive Director of the Cybersecurity and Privacy Institute, and affiliate faculty at the Center for Law, Innovation and Creativity (CLIC). His research is primarily in the areas of distributed systems and networking, with a recent focus on privacy, security, transparency, and mobile systems.

* <a href="https://www.khoury.northeastern.edu/people/daniel-j-dubois/">Dr Daniel Dubois</a> is an Associate Research Scientist at Northeastern University, his research is rooted in software engineering, with a current focus on IoT privacy. He maintains the Mon(IoT)r Lab testbed, which provides an IoT monitoring infrastructure to four research institutions.  


## NEWS
* Our paper, describing the methodology and results, “Blocking Without Breaking: Identification and Mitigation of Non-Essential IoT Traffic” has been accepted to the Privacy Enhancing Technologies Symposium <a href="https://petsymposium.org/2021/paperlist.php">(PETS 2021)</a>. More details [here.](https://moniotrlab.ccis.neu.edu/publications/pets21/)

* Our project won one of the Top 5 spots in the <a href="https://telekom-challenge.com/">Telekom Challenge</a> amongst 180 startup teams around the world. 

<a href="https://telekom-challenge.com/"><img src="https://raw.githubusercontent.com/IoTrim/iotrimlist/master/telekom.png" width="500"/></a>


