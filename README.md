# IoTrimmer Project 
This site contains a <a href="https://github.com/IoTrim/iotrimlist">set of non-required destinations list</a> from 31 consumer IoT devices and the software for producing the list. The list is created using a methodology for determining non-required destinations by automatically executing IoT device functions and determining the execution outcome while blocking selected destinations.

<a href="https://github.com/IoTrim/iotrimlist/"><img src="https://raw.githubusercontent.com/IoTrim/iotrimlist/master/iotrim.png" width="500"/></a>

## IoTrim

IoT devices offer multiple types of functionality; however, for this list, we select only the main functions for every IoT device under test. However, from preliminary experiments we have seen that most devices use the same destinations for different functions. 

The list contains 4 columns: 

* device: the device under test
* destination: the non-required destination 
* party: destination’s party type (first party, third, support)
     - First party: destination related to the device manufacturer.
     - Support party: destination that is not a first party and is responsible for providing remote computation.
     - Third party: destination that is not a First party or a Support party. 
* grouped: to facilitate analysis and streamline blocklists, we developed a strategy to group destinations thet use different DNS names and IP addresses for each replica. 

## IoTrigger and IoTrimmer

<img src="https://raw.githubusercontent.com/IoTrim/iotrimlist/master/system.png" width="1000"/>

We release the testing system <a href="https://github.com/IoTrim/IoTrigger">(IoTrigger)</a> and the blocking system <a href="https://github.com/IoTrim/IoTrimmer">(IoTrimmer)</a> that use our method for building the required and non-required destinations list <a href="https://github.com/IoTrim/iotrimlist">(IoTrim list)</a>, and use it to block non-essential traffic.

## NEWS
* Our paper, describing the methodology and results, “Blocking without Breaking: Identification and Mitigation of Non-Essential IoT Traffic” has been accepted to the Privacy Enhancing Technologies Symposium <a href="https://petsymposium.org/2021/paperlist.php">(PETS 2021)</a>.

<a href="https://petsymposium.org/2021"><img src="https://raw.githubusercontent.com/IoTrim/iotrimlist/master/pets.png" width="500"/></a>

<u>About this publication</u>

Title: Blocking without Breaking: Identification and Mitigation of Non-Essential IoT Traffic

Authors: Anna Maria Mandalari (Imperial College London), Daniel J. Dubois (Northeastern University), Roman Kolcun (Imperial College London), Muhammad Talha Paracha (Northeastern University), Hamed Haddadi (Imperial College London), and David Choffnes (Northeastern University)

Download Full Text (<a href="https://arxiv.org/abs/2105.05162">PDF</a>)

Citation:
@inproceedings{mandalari-pets21,

title={Blocking without Breaking: Identification and Mitigation of Non-Essential IoT Traffic},

author={Mandalari, Anna Maria and Dubois, Daniel J.and Kolcun, Roman and Paracha, Muhammad Talha and Haddadi, Hamed and Choffnes, David},

booktitle={Proc. of the Privacy Enhancing Technologies Symposium (PETS)},

year={2021}

}


* Our project won one of the Top 10 spots in the <a href="https://telekom-challenge.com/">Telekom Challenge</a> amongst 180 startup teams around the world. 

<a href="https://telekom-challenge.com/"><img src="https://raw.githubusercontent.com/IoTrim/iotrimlist/master/telekom.png" width="500"/></a>
