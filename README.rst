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
`This jupyter notebook/ <https://github.com/SSCP2021-group-9/hiPSC-CMs-ionic-current-block-detecion/blob/main/classify_AP.ipynb/>`_ contains 

Explainable AI code:
--------------------

`This jupyter notebook/ <https://github.com/SSCP2021-group-9/hiPSC-CMs-ionic-current-block-detecion/blob/main/sscp-explainable-ai.ipynb/>`_ shows how we LIME-models to explain the predictions of the CNN model


