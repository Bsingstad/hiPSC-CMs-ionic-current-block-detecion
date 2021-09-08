***************************************
hiPSC-CMs-ionic-current-block-detecion
***************************************

Identifying ionic channel block in a virtual cardiomyocyte population using machine learning classifiers




Data:
=====
The data set (data.h5) used in this study contains 4582 cytosolic calsium (Ca2+) and transmembrane voltage (Vt) signals from a simulated cardiomyocyte (CM) without ion channel block and 4582 Ca2+ and Vt signals from CM with ion channel block. The 
the Vt and Ca2+ signals from each ion blocked case was subtracted from the Vt and Ca2+ signals from the control case.







.. image:: https://github.com/SSCP2021-group-9/hiPSC-CMs-ionic-current-block-detecion/blob/main/img/v_control.png
**Figure 1:** An example of transmembrane voltage signal from a simulated cardiomyocyte without any ion channel block 

.. image:: https://github.com/SSCP2021-group-9/hiPSC-CMs-ionic-current-block-detecion/blob/main/img/v_drug.png
**Figure 2:** An example of transmembrane voltage signal from a simulated cardiomyocyte with any ion channel block 

.. image:: https://github.com/SSCP2021-group-9/hiPSC-CMs-ionic-current-block-detecion/blob/main/img/Vdrug-Vcontrol.png
**Figure 3:** The transmembrane voltage signal from Figure 2 subtracted by the transmembrane voltage signal in Figure 1




Jupyter Notebooks:
==================

Training and cross-validation:
-----------------------------
`https://datasets.simula.no/kvasir-instrument/ <https://github.com/SSCP2021-group-9/hiPSC-CMs-ionic-current-block-detecion/blob/main/classify_AP.ipynb/>`_
The two jupyter notebooks in this repository give you a fundament for staring the development of the polyp and instrument segmentation tasks. As a baseline model we have provided a Unet build with Keras. Finally, we run the model inside a 10-fold cross-validation loop and we encourage the participants to also use som kind of resampling methods when reporting the results on the development set in the final paper to Nordic Machine Intelligence. 

Run the code:
-------------

You can run the code by forking and clone this repository. Then download the datasets and extract them to this cloned repository.
The folder structrure should look like this: 
    
 | ├── hyperkvasir-starter-code.ipynb
 | ├── kvasir-instrument-starter-code.ipynb
 | ├── kvasir-instrument         
 | │   ├── bboxes.json
 | │   ├── test.txt
 | │   ├── train.txt
 | │   ├── images
 | │   └── masks
 | ├── kvasir-SEG        
 | │   ├── kavsir_bboxes.json
 | │   ├── test.txt
 | │   ├── train.txt
 | │   ├── images
 | │   └── masks

 
Finally, you should pip install the necessary python packages and then you can run the code!

References:
===========

.. [#] Debesh Jha, Pia H. Smedsrud, Michael A. Riegler, Pål Halvorsen, Dag Johansen, Thomas de Lange, and Håvard D. Johansen, Kvasir-SEG: A Segmented Polyp Dataset, In Proceedings of the ternational conference on Multimedia Modeling, Republic of Korea, 2020.
.. [#] Jha, Debesh, et al. “Kvasir-instrument: Diagnostic and Therapeutic Tool Segmentation Dataset in Gastrointestinal Endoscopy.” OSF Preprints, 15 Aug. 2020. Web



