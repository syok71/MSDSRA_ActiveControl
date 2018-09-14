The codes show how to evaluate "Multi-Scale Dynamic System Reliability Analysis of Actively-Controlled Structures subject to Earthquake Excitations".
The codes are based on the paper "Seung-Min Kim, Seung-Yong Ok and Junho Song" submitted to KSCE Journal of Civil Engineering. 
The paper's full reference information is as follows:
  - Kim, S.-M., Ok, S.-Y. and J. Song (2018). Multi-Scale Dynamic System Reliability Analysis of Actively-Controlled Structures subject to Earthquake Excitations, KSCE Journal of Civil Engineering.

To estimate the proposed approach, multi-scale dynamic system reliability analysis has been developed. 

All programs are perfomed based on the MATLAB progam.
In order to run the progrom, it requires FERUM(Finite Element Reliability Using Matlab) being installed. 
For more information on FERUM, please visit http://www.ce.berkeley.edu/projects/ferum/.
The code also uses Genz algorithm that is already included in the code with a file name "qsimvnv.m". 
For more information on FERUM, please visit http://www.math.wsu.edu/faculty/genz/homepage.
 
How to use the developed Matlab code:

The code consists of 3 parts such as (1) Lower-level system reliability analysis for floor failure probability, (2) Joint system reliability analysis for failure probability between two floors and (3) Higher-level system reliability analysis for failure probability of the structural system.

1. Unzip "Pf_Flrs_Active_Mixed.zip" into a directory named as "Sys".
2. Install FERUM in the "Sys" directory. Then, you can have "ferumcore" directory with sub-directories of "Distribution and Sensitivities", "Inverse Form", "Sorm CF", "Sorm PF" and "Tvedt" in it. 
3. Move a "user_lsf.m" file into "ferumcore" directory. 
4. Then, run "Run_Pf_1Flr_Active_Mixed.m", "Run_Pf_2Flr_Active_Mixed.m" and "Run_Pf_3Flr_Active_Mixed.m" sequentially.  Each file computes the lower-level failure probability of each floor.
5. Thereafter, unzip "Pf_Joint_Active_Mixed.zip" into a directory named as "Sys_joint".
6. Then, run "Run_JointPf_12Flors_Active_Mixed.m", "Run_JointPf_12Flors_Active_Mixed.m" and "Run_JointPf_12Flors_Active_Mixed.m" in sequence. Each file computes the joint failure probabilities between two floors. 
7. Then, unzip "Pf_Sys_Active_Mixed.zip" into a directory named as "Sys_rho". 
8. Finally, run "Run_SysPf_123Flrs_Active_Mixed.m" to compute the system reliability or failure probability of the system.
 
Remark:

The code is to compute the system reliability of actively-controlled structural system under the uncertainties in both system and loading. Therefore, note that we need to modify the code in order to evaluate the system reliability analysis of the original structure without active control system, and the case of uncertainty in earthquake excitations only. In other words, the study consists of 4 parts such as (1) Original System with Loading Uncertainty, (2) Original Sysmtem with Loading and System Uncertainties, (3) Active Control System with Loading Uncertainty and (4) Active Control System with Loading and System Uncertainties. Here, we only upload the last one that is Active Control System with Loading and System Uncertainties. The others can be modified easily from the code by removing the active control system part and system uncertainty part. 

Acknowledgement:
 
The authors would like to thank Prof. Terje Haukaas who is the code developer of FERUM, respectively.
The authors also would like to thank Prof. Alan Genz who is the code developer of Genz algorithm. 
