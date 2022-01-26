
### Evaluation Folder
This folder contains codes used for synthetic data evaluation and real-world RCT data evaluation. 
For synthetic data evaluation we adopted ITE measurement proposed in https://arxiv.org/abs/1901.10550 
and the result is shown in Section 5.1. For offline test on real-word data, we adopte PMG method described in section 3,
corresponding to the result in Section 5.2:

    run Simulation_analysis.py to calculate ITE.
    run Offline_test.py to calculate PMG.

*Note: Due to the privacy nature of this real-world offine test dataset, currently we are not able to disclose the complete data used in this test until we get authorization. Offline_test.py only provides the sample code to calculate percentage mean gain. NOT FOR REPRODUCE THE RESULT** in Section 5.2*
