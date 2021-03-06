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

## IoTrimmer and IoTrigger

<img src="https://raw.githubusercontent.com/IoTrim/iotrimlist/master/system.png" width="1000"/>

We release the blocking system <a href="https://github.com/IoTrim/IoTrimmer">(IoTrimmer)</a> that uses the required and non-required destinations list <a href="https://github.com/IoTrim/iotrimlist">(IoTrim list)</a> to block non-essential traffic.

IoTrigger is the testing system, our method for building the required and non-required destinations list (see the <a href="https://arxiv.org/abs/2105.05162">pre-print paper.</a>)

## TEAM
Our team has extensive experience in the area of privacy for Internet of Things (IoT) devices. To date, the software artifacts of our research team have produced reports and datasets that informed additional research, policy debates, and regulators. During the past 2 years, we worked on the problem of modeling and evaluating adaptation strategies based on measurements techniques for IoT devices. All the research experience above resulted in peer-reviewed papers, published in top tier scientific conferences and funded research projects.

* <a href="https://haddadi.github.io/">Professor Hamed Haddadi</a> is an Associate Professor in Human-Centred Systems and the Director of Postgraduate Studies at the Dyson School of Design Engineering, at the Faculty of Engineering at Imperial College London. He is a Security Science Fellow of the Institute for Security Science and Technology and of the Data Science Institute. He is also a Visiting Professor at Brave Software where he works on developing privacy-preserving protocols.
 
* <a href="https://www.imperial.ac.uk/people/anna-maria.mandalari">Dr Anna Maria Mandalari</a> is a Research Associate at Imperial College, her research interests are related to IoT, privacy, large-scale Internet measurements, Internet measurement platforms, middleboxes and new Internet protocols. 

* <a href="https://david.choffnes.com/">Professor David Choffnes</a> is an Associate Professor at Northeastern University, Executive Director of the Cybersecurity and Privacy Institute, and affiliate faculty at the Center for Law, Innovation and Creativity (CLIC). His research is primarily in the areas of distributed systems and networking, with a recent focus on privacy, security, transparency, and mobile systems.

* <a href="https://www.khoury.northeastern.edu/people/daniel-j-dubois/">Dr Daniel Dubois</a> is an Associate Research Scientist at Northeastern University, his research is rooted in software engineering, with a current focus on IoT privacy. He maintains the Mon(IoT)r Lab testbed, which provides an IoT monitoring infrastructure to four research institutions.  


## NEWS
* Our paper, describing the methodology and results, “Blocking Without Breaking: Identification and Mitigation of Non-Essential IoT Traffic” has been accepted to the Privacy Enhancing Technologies Symposium <a href="https://petsymposium.org/2021/paperlist.php">(PETS 2021)</a>.

<a href="https://petsymposium.org/2021"><img src="https://raw.githubusercontent.com/IoTrim/iotrimlist/master/pets.png" width="500"/></a>

<u>About this publication</u>

-- Title: Blocking Without Breaking: Identification and Mitigation of Non-Essential IoT Traffic

-- Authors: Anna Maria Mandalari (Imperial College London), Daniel J. Dubois (Northeastern University), Roman Kolcun (Imperial College London), Muhammad Talha Paracha (Northeastern University), Hamed Haddadi (Imperial College London), and David Choffnes (Northeastern University)

-- Download Full Text (<a href="https://arxiv.org/abs/2105.05162">PDF</a>)

-- Citation:
@inproceedings{mandalari-pets21,

title={Blocking Without Breaking: Identification and Mitigation of Non-Essential IoT Traffic},

author={Mandalari, Anna Maria and Dubois, Daniel J.and Kolcun, Roman and Paracha, Muhammad Talha and Haddadi, Hamed and Choffnes, David},

booktitle={Proc. of the Privacy Enhancing Technologies Symposium (PETS)},

year={2021}

}


* Our project won one of the Top 10 spots in the <a href="https://telekom-challenge.com/">Telekom Challenge</a> amongst 180 startup teams around the world. 

<a href="https://telekom-challenge.com/"><img src="https://raw.githubusercontent.com/IoTrim/iotrimlist/master/telekom.png" width="500"/></a>


