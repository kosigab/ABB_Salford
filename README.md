# ABB_Salford
This Git repository contains a comprehensive script designed for ABB Robot Studio, showcasing the step-by-step process of using the IRB1200 robot to write on a virtual paper using a specialized pen tool. 
//.........................//


MODULE Module1
       
    TASK PERS tooldata toolPen:=[TRUE,[[100,0,20],[0.653281482,0.27059805,-0.653281482,-0.27059805]],[0.1,[50,0,10],[1,0,0,0],0,0,0]];
    TASK PERS wobjdata WkObj_tilt_paper:=[FALSE,TRUE,"",[[403.87242208,428.126413661,0.1],[0.765935658,-0.001715767,0.001440186,-0.64291333]],[[0,0,0],[1,0,0,0]]];
    TASK PERS wobjdata WkObj_paper:=[FALSE,TRUE,"",[[459.660289856,-90.375541036,0.1],[0.711712441,0,0,-0.702470925]],[[0,0,0],[1,0,0,0]]];
    TASK PERS wobjdata WkObj_paper_2:=[FALSE,TRUE,"",[[234.420012927,103.808224608,3],[0.710975028,0,0,-0.703217256]],[[0,0,0],[1,0,0,0]]];
    
    CONST robtarget Target_10:=[[93.567,105.118,0.471],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_10_up:=[[93.567,105.118,15.471],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_20:=[[58.348,69.936,0.313],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_30:=[[23.568,104.807,0.47],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_40:=[[58.181,139.933,0.627],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_50:=[[138.972,139.962,0.627],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_50_up:=[[138.972,139.962,15.627],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_60:=[[118.553,159.572,0.715],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_70:=[[138.416,179.961,0.806],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_80:=[[177.943,179.974,0.806],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_90:=[[178.556,139.975,0.627],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_100:=[[203.558,134.755,0.604],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_100_up:=[[203.558,134.755,15.604],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_110:=[[203.578,74.984,0.336],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_120:=[[258.558,135.002,0.605],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_130:=[[258.578,75.002,0.336],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_140:=[[53.514,125.34,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_140_up:=[[53.514,125.34,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_150:=[[33.262,145.018,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_160:=[[13.517,125.103,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_170:=[[53.431,85.323,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_180:=[[33.191,65.021,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_190:=[[13.435,85.316,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_190_up:=[[13.435,85.316,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_200:=[[59.391,64.965,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_200_up:=[[59.391,64.965,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_210:=[[78.629,144.643,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_220:=[[98.391,64.883,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_220_up:=[[98.391,64.883,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_230:=[[90.778,95.608,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_230_up:=[[90.778,95.608,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_240:=[[66.144,95.706,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_240_up:=[[66.144,95.706,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_250:=[[104.559,144.871,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_250_up:=[[104.559,144.871,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_260:=[[103.588,64.873,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_270:=[[133.391,64.81,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_270_up:=[[133.391,64.81,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_320:=[[163.474,104.53,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_320_up:=[[163.474,104.53,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_280:=[[139.391,64.798,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_280_up:=[[139.391,64.798,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_290:=[[138.848,144.799,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_300:=[[168.558,144.737,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_300_up:=[[168.558,144.737,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_310:=[[138.475,104.786,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_310_up:=[[138.475,104.786,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_330:=[[173.532,130.077,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_330_up:=[[173.532,130.077,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_340:=[[173.423,80.229,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_350:=[[188.569,64.696,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_360:=[[203.422,79.653,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_370:=[[203.526,129.395,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_380:=[[188.966,144.688,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_390:=[[208.558,144.653,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_390_up:=[[208.558,144.653,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_400:=[[238.516,124.458,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_410:=[[209.477,105.664,0.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_410_up:=[[209.477,105.664,15.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_420:=[[209.391,64.651,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_420_up:=[[209.391,64.651,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_430:=[[217.983,104.639,0.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_430_up:=[[217.983,104.639,15.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_440:=[[237.92,64.591,0.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_440_up:=[[237.92,64.591,15.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_880:=[[218.659,144.631,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_450:=[[243.584,64.58,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_450_up:=[[243.584,64.58,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_460:=[[243.438,144.579,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_470:=[[283.472,104.122,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_480:=[[45.896,120.703,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_480_up:=[[45.896,120.703,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_490:=[[24.977,133.794,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_500:=[[11.172,113.371,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_510:=[[10.888,100.881,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_520:=[[24.63,80.457,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_530:=[[45.442,92.811,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_540:=[[45.624,100.801,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_550:=[[34.306,100.675,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_550_up:=[[34.306,100.675,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_560:=[[54.893,80.211,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_560_up:=[[54.893,80.211,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_570:=[[73.567,133.293,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_580:=[[91.777,80.159,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_580_up:=[[91.777,80.159,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_590:=[[85.638,97.852,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_590_up:=[[85.638,97.852,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_600:=[[61.417,98.204,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_600_up:=[[61.417,98.204,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_610:=[[103.157,80.344,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_610_up:=[[103.157,80.344,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_620:=[[124.196,80.104,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_630:=[[135.562,92.548,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_640:=[[124.497,107.445,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_650:=[[103.544,107.691,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_660:=[[103.345,133.097,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_670:=[[124.045,132.97,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_680:=[[135.627,119.521,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_690:=[[151.413,79.024,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_690_up:=[[151.413,79.024,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_700:=[[151.856,132.89,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_710:=[[173.039,132.507,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_720:=[[184.456,119.407,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_730:=[[172.412,107.013,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_740:=[[151.728,107.485,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_740_up:=[[151.728,107.485,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_750:=[[167.969,107.12,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_750_up:=[[167.969,107.12,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_760:=[[183.941,79.582,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_760_up:=[[183.941,79.582,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_770:=[[200.091,79.02,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_770_up:=[[200.091,79.02,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_780:=[[200.125,131.97,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_780_up:=[[200.125,131.97,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_790:=[[249.142,132.294,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_790_up:=[[249.142,132.294,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_800:=[[218.62,132.453,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_810:=[[217.893,79.55,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_820:=[[248.627,79.332,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_820_up:=[[248.627,79.332,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_830:=[[218.231,107.276,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_830_up:=[[218.231,107.276,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_840:=[[236.836,107.366,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_840_up:=[[236.836,107.366,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

   
    CONST robtarget Target_920:=[[37.793,82.537,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_910:=[[16.28,87.423,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_900:=[[15.554,125.157,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_890:=[[36.188,132.642,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    
    CONST robtarget Target_860:=[[261.931,79.067,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    
    CONST robtarget Target_870:=[[289.646,78.964,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
        CONST robtarget Target_870_up:=[[289.646,78.964,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];

    CONST robtarget Target_850:=[[262.426,132.517,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget Target_850_up:=[[262.426,132.517,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget s1up:=[[53.514,125.34,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget s1:=[[53.514,125.34,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget s2:=[[33.262,145.018,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget s3:=[[13.517,125.103,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget s4:=[[53.431,85.323,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget s5:=[[33.191,65.021,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget s6:=[[13.435,85.316,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget s6up:=[[13.435,85.316,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a1up:=[[59.391,64.965,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a1:=[[59.391,64.965,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a2:=[[78.629,144.643,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a3:=[[98.391,64.883,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a3up:=[[98.391,64.883,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a4up:=[[90.778,95.608,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a4:=[[90.778,95.608,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a5:=[[66.144,95.706,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a5up:=[[66.144,95.706,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget l1up:=[[104.559,144.871,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget l1:=[[104.559,144.871,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget l2:=[[103.588,64.873,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget l3:=[[133.391,64.81,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget l3up:=[[133.391,64.81,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget f1up:=[[139.391,64.798,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget f1:=[[139.391,64.798,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget f2:=[[138.848,144.799,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget f3:=[[168.558,144.737,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget f3up:=[[168.558,144.737,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget f4up:=[[138.475,104.786,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget f4:=[[138.475,104.786,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget f5:=[[163.474,104.53,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget f5up:=[[163.474,104.53,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget o1up:=[[173.532,130.077,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget o1:=[[173.532,130.077,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget o2:=[[173.423,80.229,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget o3:=[[188.569,64.696,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget o4:=[[203.422,79.653,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget o5:=[[203.526,129.395,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget o6:=[[188.966,144.688,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r1up:=[[208.558,144.653,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r1:=[[208.558,144.653,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r7:=[[218.659,144.631,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r2:=[[238.516,124.458,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r5:=[[217.983,104.639,0.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r3:=[[209.477,105.664,0.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r3up:=[[209.477,105.664,15.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r4:=[[209.391,64.651,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r4up:=[[209.391,64.651,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r5up:=[[217.983,104.639,15.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r6:=[[237.92,64.591,0.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r6up:=[[237.92,64.591,15.01],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget d1up:=[[243.584,64.58,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget d1:=[[243.584,64.58,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget d2:=[[243.438,144.579,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget d3:=[[283.472,104.122,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g1up:=[[45.896,120.703,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g1:=[[45.896,120.703,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g9:=[[36.188,132.642,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g2:=[[24.977,133.794,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g10:=[[15.554,125.157,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g3:=[[11.172,113.371,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g4:=[[10.888,100.881,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g11:=[[16.28,87.423,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g5:=[[24.63,80.457,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g12:=[[37.793,82.537,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g6:=[[45.442,92.811,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g7:=[[45.624,100.801,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g8:=[[34.306,100.675,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget g8up:=[[34.306,100.675,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a1up_:=[[54.893,80.211,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a1_:=[[54.893,80.211,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a2_:=[[73.567,133.293,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a3_:=[[91.777,80.159,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a3up_:=[[91.777,80.159,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a4up_:=[[85.638,97.852,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a4_:=[[85.638,97.852,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a5_:=[[61.417,98.204,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget a5up_:=[[61.417,98.204,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget b1up:=[[103.157,80.344,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget b1:=[[103.157,80.344,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget b2:=[[124.196,80.104,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget b3:=[[135.562,92.548,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget b4:=[[124.497,107.445,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget b5:=[[103.544,107.691,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget b8:=[[135.627,119.521,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget b7:=[[124.045,132.97,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget b6:=[[103.345,133.097,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r1up_:=[[151.413,79.024,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r1_:=[[151.413,79.024,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r2_:=[[151.856,132.89,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r3_:=[[173.039,132.507,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r4_:=[[184.456,119.407,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r5_:=[[172.412,107.013,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r6_:=[[151.728,107.485,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r6up_:=[[151.728,107.485,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r7up_:=[[167.969,107.12,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r7_:=[[167.969,107.12,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r8_:=[[183.941,79.582,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget r8up_:=[[183.941,79.582,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget i1up:=[[200.091,79.02,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget i1:=[[200.091,79.02,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget i2:=[[200.125,131.97,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget i2up:=[[200.125,131.97,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget e1up:=[[249.142,132.294,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget e1:=[[249.142,132.294,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget e2:=[[218.62,132.453,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget e3:=[[217.893,79.55,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget e4:=[[248.627,79.332,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget e4up:=[[248.627,79.332,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget e5up:=[[218.231,107.276,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget e5:=[[218.231,107.276,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget e6:=[[236.836,107.366,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget e6up:=[[236.836,107.366,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget l1up_:=[[262.426,132.517,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget l1_:=[[262.426,132.517,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget l2_:=[[261.931,79.067,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget l3_:=[[289.646,78.964,0],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget l3up_:=[[289.646,78.964,15],[1,0,0,0],[-1,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget circle1up:=[[93.567,105.118,15.471],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget circle1:=[[93.567,105.118,0.471],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget circle2:=[[58.348,69.936,0.313],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget circle3:=[[23.568,104.807,0.47],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget circle4:=[[58.181,139.933,0.627],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget dShape1up:=[[138.972,139.962,15.627],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget dShape1:=[[138.972,139.962,0.627],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget dShape2:=[[118.553,159.572,0.715],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget dShape3:=[[138.416,179.961,0.806],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget dShape4:=[[177.943,179.974,0.806],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget dShape5:=[[178.556,139.975,0.627],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget sqaure1up:=[[203.558,134.755,15.604],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget sqaure1:=[[203.558,134.755,0.604],[1,0,0,0],[0,0,0,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget sqaure2:=[[203.578,74.984,0.336],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget sqaure4:=[[258.578,75.002,0.336],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];
    CONST robtarget sqaure3:=[[258.558,135.002,0.605],[1,0,0,0],[0,-2,1,0],[9E+09,9E+09,9E+09,9E+09,9E+09,9E+09]];



PROC main()
    TPErase;
    TPWrite"ABB RobotStudio practicals - Gabriel Ejimonu.";
    TPReadFK reg1,"What would you like to draw/write?","Shapes","Salford","Name","All of the above",stEmpty;
    TEST reg1
    CASE 1:
    SHAPES;
    CASE 2:
    SALFORD;
    CASE 3:
    NAME;
    CASE 4:
    SHAPES;
    SALFORD;
    NAME;
    ENDTEST
         
      
      
    ENDPROC
     PROC SHAPES()
        ShapeCircle;
        WaitTime 2;
        ShapeD;
         WaitTime 2;
        ShapeSquare;
         WaitTime 2;
    ENDPROC
    PROC SALFORD()
        Letter_S;
        Letter_A; 
        Letter_L;
        Letter_F;
        Letter_O;
        Letter_R;
        Letter_D;
      
     
    ENDPROC
    PROC NAME()
        Letter_G;
        Letter_A_2;
        Letter_B;
        Letter_R_2;
        Letter_I;
        Letter_E;
        Letter_L_2;
    ENDPROC
    PROC ShapeCircle()
        MoveJ circle1up,v1000,fine,toolPen\WObj:=WkObj_tilt_paper;

        MoveL circle1,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        MoveC circle2,circle3,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        MoveC circle4,circle1,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        
        MoveJ circle1up,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        
        
      

    ENDPROC
    PROC ShapeD()
        MoveJ dShape1up,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        MoveL dShape1,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        MoveC dShape2,dShape3,v100,fine,toolPen\WObj:=WkObj_tilt_paper;      
        MoveL dShape4,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        MoveL dShape5,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        MoveL dShape1,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
         MoveL dShape1up,v100,fine,toolPen\WObj:=WkObj_tilt_paper;

    ENDPROC
    PROC ShapeSquare()
        MoveJ sqaure1up,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        MoveL sqaure1,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        MoveL sqaure2,v100,fine,toolPen\WObj:=WkObj_tilt_paper;     
        MoveL sqaure4,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        MoveL sqaure3,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
        MoveL sqaure1,v100,fine,toolPen\WObj:=WkObj_tilt_paper;
         MoveL sqaure1up,v100,fine,toolPen\WObj:=WkObj_tilt_paper;

    ENDPROC
    PROC Letter_S()
        MoveJ s1up,v1000,fine,toolPen\WObj:=WkObj_paper;
        MoveL s1,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveC s2,s3,v100,fine,toolPen\WObj:=WkObj_paper;       
        MoveL s4,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveC s5,s6,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL s6,v100,fine,toolPen\WObj:=WkObj_paper;
           MoveL s6up,v100,fine,toolPen\WObj:=WkObj_paper;

    ENDPROC
    PROC Letter_A()
        MoveJ a1up,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL a1,v100,fine,toolPen\WObj:=WkObj_paper;
     
        MoveL a2,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL a3,v100,fine,toolPen\WObj:=WkObj_paper;
          MoveL a3up,v100,fine,toolPen\WObj:=WkObj_paper;
            MoveL a4up,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL a4,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL a5,v100,fine,toolPen\WObj:=WkObj_paper;
          MoveL a5up,v100,fine,toolPen\WObj:=WkObj_paper;

    ENDPROC
    PROC Letter_L()
          MoveJ l1up,v100,fine,toolPen\WObj:=WkObj_paper;

        MoveL l1,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL l2,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL l3,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL l3up,v100,fine,toolPen\WObj:=WkObj_paper;

    ENDPROC
    PROC Letter_F()
               MoveJ f1up,v100,fine,toolPen\WObj:=WkObj_paper;

        MoveL f1,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL f2,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL f3,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL f3up,v100,fine,toolPen\WObj:=WkObj_paper;
                MoveJ f4up,v100,fine,toolPen\WObj:=WkObj_paper;

        MoveL f4,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL f5,v100,fine,toolPen\WObj:=WkObj_paper;
                MoveL f5up,v100,fine,toolPen\WObj:=WkObj_paper;


    ENDPROC
    PROC Letter_O()
          MoveJ o1up,v100,fine,toolPen\WObj:=WkObj_paper;

        MoveL o1,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL o2,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveC o3,o4,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL o5,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveC o6,o1,v100,fine,toolPen\WObj:=WkObj_paper;
        
        MoveL o1up,v100,fine,toolPen\WObj:=WkObj_paper;

    ENDPROC
    PROC Letter_R()
        
        MoveJ r1up,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL r1,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL r7,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveC r2,r5,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL r3,v100,fine,toolPen\WObj:=WkObj_paper;

            MoveL r3up,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveJ r1up,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL r1,v100,fine,toolPen\WObj:=WkObj_paper;
      
        MoveL r4,v100,fine,toolPen\WObj:=WkObj_paper;
            MoveL r4up,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL r5up,v100,fine,toolPen\WObj:=WkObj_paper;

        MoveL r5,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL r6,v100,fine,toolPen\WObj:=WkObj_paper;
                MoveL r6up,v100,fine,toolPen\WObj:=WkObj_paper;


    ENDPROC
    PROC Letter_D()
        MoveL d1up,v100,fine,toolPen\WObj:=WkObj_paper;

        MoveL d1,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL d2,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveC d3,d1,v100,fine,toolPen\WObj:=WkObj_paper;
        MoveL d1up,v100,fine,toolPen\WObj:=WkObj_paper;

    ENDPROC
    PROC Letter_G()
                MoveJ g1up,v1000,fine,toolPen\WObj:=WkObj_paper_2;

        MoveL g1,v100,fine,toolPen\WObj:=WkObj_paper_2;
                MoveC g9,g2,v100,fine,toolPen\WObj:=WkObj_paper_2;

        MoveC g10,g3,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL g4,v100,fine,toolPen\WObj:=WkObj_paper_2;
       
        MoveC g11,g5,v100,fine,toolPen\WObj:=WkObj_paper_2;
                MoveC g12,g6,v100,fine,toolPen\WObj:=WkObj_paper_2;

        MoveL g7,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL g8,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL g8up,v100,fine,toolPen\WObj:=WkObj_paper_2;
        
      

    ENDPROC
    PROC Letter_A_2()
            MoveJ a1up_,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL a1_,v100,fine,toolPen\WObj:=WkObj_paper_2;
     
        MoveL a2_,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL a3_,v100,fine,toolPen\WObj:=WkObj_paper_2;
          MoveL a3up_,v100,fine,toolPen\WObj:=WkObj_paper_2;
            MoveL a4up_,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL a4_,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL a5_,v100,fine,toolPen\WObj:=WkObj_paper_2;
          MoveL a5up_,v100,fine,toolPen\WObj:=WkObj_paper_2;
          
         

    ENDPROC
    PROC Letter_B()
                MoveJ b1up,v100,fine,toolPen\WObj:=WkObj_paper_2;

        MoveL b1,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL b2,v100,fine,toolPen\WObj:=WkObj_paper_2;
        
        MoveC b3,b4,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL b5,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL b4,v100,fine,toolPen\WObj:=WkObj_paper_2;

        MoveC b8,b7,v100,fine,toolPen\WObj:=WkObj_paper_2;
        
        MoveL b6,v100,fine,toolPen\WObj:=WkObj_paper_2;
         MoveL b1,v100,fine,toolPen\WObj:=WkObj_paper_2;
           MoveL b1up,v100,fine,toolPen\WObj:=WkObj_paper_2;
        

    ENDPROC
    PROC Letter_R_2()
                MoveJ r1up_,v100,fine,toolPen\WObj:=WkObj_paper_2;

        MoveL r1_,v100,fine,toolPen\WObj:=WkObj_paper_2;
        
        MoveL r2_,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL r3_,v100,fine,toolPen\WObj:=WkObj_paper_2;
       
        MoveC r4_,r5_,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL r6_,v100,fine,toolPen\WObj:=WkObj_paper_2;
          MoveL r6up_,v100,fine,toolPen\WObj:=WkObj_paper_2;
              MoveL r7up_,v100,fine,toolPen\WObj:=WkObj_paper_2;

        MoveL r7_,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL r8_,v100,fine,toolPen\WObj:=WkObj_paper_2;
              MoveL r8up_,v100,fine,toolPen\WObj:=WkObj_paper_2;


    ENDPROC
    PROC Letter_I()
                MoveJ i1up,v100,fine,toolPen\WObj:=WkObj_paper_2;

        MoveL i1,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL i2,v100,fine,toolPen\WObj:=WkObj_paper_2;
                MoveL i2up,v100,fine,toolPen\WObj:=WkObj_paper_2;


    ENDPROC
    PROC Letter_E()
                        MoveJ e1up,v100,fine,toolPen\WObj:=WkObj_paper_2;

        MoveL e1,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL e2,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL e3,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL e4,v100,fine,toolPen\WObj:=WkObj_paper_2;
                MoveL e4up,v100,fine,toolPen\WObj:=WkObj_paper_2;
                MoveL e5up,v100,fine,toolPen\WObj:=WkObj_paper_2;

        MoveL e5,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL e6,v100,fine,toolPen\WObj:=WkObj_paper_2;
                        MoveL e6up,v100,fine,toolPen\WObj:=WkObj_paper_2;


    ENDPROC
    PROC Letter_L_2()
                MoveJ l1up_,v100,fine,toolPen\WObj:=WkObj_paper_2;

        MoveL l1_,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL l2_,v100,fine,toolPen\WObj:=WkObj_paper_2;
        MoveL l3_,v100,fine,toolPen\WObj:=WkObj_paper_2;
                MoveL l3up_,v100,fine,toolPen\WObj:=WkObj_paper_2;


    ENDPROC
ENDMODULE
