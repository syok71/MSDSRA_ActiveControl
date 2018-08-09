The codes show how to evaluate "Multi-Scale Dynamic System Reliability Analysis of Actively-Controlled Structures subject to Earthquake Excitations".

The codes are based on the paper "Seung-Min Kim, Seung-Yong Ok and Junho Song" Presented at KSCE Journal of Civil Engineering. 
% The paper¡¯s full reference information is as follows:

% Kim, S.-M., Ok, S.-Y. and J. Song (2018). Multi-Scale Dynamic System Reliability Analysis of Actively-Controlled Structures subject to Earthquake Excitations, KSCE Journal of Civil Engineering.
% DOI: https://doi.org/10.1016/j.ress.2018.01.005

To estimate the proposed approach, multi-scale dynamic system reliability analysis is developed. 
All programs are perfomed based on the MATLAB progam and incorporate a tool box of Finite Element Reliability Using Matlab (FERUM), directly. 
For more information on FERUM, please visit http://www.ce.berkeley.edu/projects/ferum/.

How to use the developed Matlab code
1. Run "comp_Pf_MDOF_Active_first.m", "~second.m" and "~third.m" for estimating the failure probabilities of each floor. 
2. Then, run "comp_Pf_Mixed_MDOF_first_second_joint.m", "~first_third_joint.m" and "~second_third_joint.m".
3. Then, run "run_rho.m" to find out the correlation between floors.
4. Finally, run "run_Sys.m" to compute the system reliability or failure probability of the system.

Remark:
- One could modify this function to solve other problems of interest.
- Please note that we need to modify the code in order to evaluate the system reliability analysis of the original structure without active control system, and the cases of uncertainties in system parameters and earthquake excitations.

Acknowledgement:
The authors would like to thank Prof. Terje Haukaas who is the code developer of FERUM, respectively.
