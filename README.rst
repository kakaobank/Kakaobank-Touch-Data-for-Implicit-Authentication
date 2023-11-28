=================================================
Kakaobank Touch Data for Implicit Authentication
=================================================

The official public anonymized data from Kakaobank for internal laboratory research and the paper 'Normalizing Flow-based Latent Space Mapping for Implicit Pattern Authentication on Mobile Devices' (Under Review).



Description & Data Schema
--------------------------
Timestamps, XY coordinates, and certain demographic characteristics of touch data collected from 6-digit number presses.

NOTICE: The number pad arrangement is shuffled randomly each time, without any inferable patterns. Therefore, the pressed numbers cannot be inferred from the XY coordinates of the data.


+------+--------------------------------------------------------------------------------------------------------------------------------+
|Column|Description                                                                                                                     |
+======+================================================================================================================================+
|A_New |Hashed Quasi-Identifier. A unique quasi-identifier is assigned, even if it refers to the same identity in some cases.           |
|      |This measure is implemented for privacy protection and is irreversible by nature, occurring during the data collection process. |
+------+--------------------------------------------------------------------------------------------------------------------------------+
|T{n}  |Timestamp of (n+1)-th touch - Timestamp of n-th touch. 'ms' is a measurement unit.                                              |
+------+--------------------------------------------------------------------------------------------------------------------------------+
|X{n}  |X coordinate of n-th touch. Normalized as a float between 0 and 1.                                                              |
+------+--------------------------------------------------------------------------------------------------------------------------------+
|Y{n}  |Y coordinate of n-th touch. Normalized as a float between 0 and 1.                                                              | 
+------+--------------------------------------------------------------------------------------------------------------------------------+
|B     |Related to the type of device.                                                                                                  |
+------+--------------------------------------------------------------------------------------------------------------------------------+
|C     |One of the demographic characteristics.                                                                                         |
+------+--------------------------------------------------------------------------------------------------------------------------------+
|D     |One of the demographic characteristics.                                                                                         |
+------+--------------------------------------------------------------------------------------------------------------------------------+

License
--------
This data is licensed under the `CC BY-NC-SA-4.0 <LICENSE>`__, quoted below.

Copyright 2023 KakaoBank Corp. https://www.kakaobank.com/

Licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License (the "License"); you may not use this data except in compliance with the License. You may obtain a copy of the License at https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode.

Unless required by applicable law or agreed to in writing, the data distributed under the License is distributed, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

Bibtex
-------
To cite this dataset, please use the following BibTex for citations:

.. code:: python
    
    @misc{kkbtouchdataimpauth,
    author = {Kakaobank},
    year = {2023},
    howpublished = {Version V1. \url{https://github.com/kakaobank/Kakaobank-Touch-Data-for-Implicit-Authentication}},
    title = {Kakaobank Touch Data for Implicit Authentication}
    }
