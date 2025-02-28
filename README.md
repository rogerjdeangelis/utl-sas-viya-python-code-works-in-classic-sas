# utl-sas-viya-python-code-works-in-classic-sas
sas viya python code works in classic sas
    %let pgm=utl-sas-viya-python-code-works-in-classic-sas;

    %stop_submission;

    sas viya python code works in classic sas

    github
    https://tinyurl.com/4v8wp2y6
    https://github.com/rogerjdeangelis/utl-sas-viya-python-code-works-in-classic-sas

    sas communities
    https://tinyurl.com/ybxv49f7
    https://communities.sas.com/t5/SAS-Programming/Proc-Python-pandas-error-on-sas-viya-4/m-p/956098#M373358

    /***********************************************************************************************************************************/
    /*                                                          |                                          |                           */
    /*          INPUT                                           |                                          |                           */
    /*  INTERNAL TO PYTHON SCRIPT                               | BASE SAS DROPDOWN TO PYTHON              |                           */
    /*  =========================                               | ============================             |                           */
    /*                                                          |                                          |                           */
    /*                                                          |                                          |                           */
    /*  want = pd.DataFrame({                                   | proc datasets lib=sd1 nolist nodetails;  | SD1.WANT                  */
    /*  "A": 1.0,                                               |  delete pywant;                          |                           */
    /*  "B": pd.Timestamp("20130102"),                          | run;quit;                                | A    B     C D   E    F   */
    /*  "C": pd.Series(1,index=list(range(4)),dtype="float32"), |                                          |                           */
    /*  "D": np.array([3]*4,dtype="int32"),                     | %utl_pybeginx;                           | 1 01/02/13 1 3 test  foo  */
    /*  "E": pd.Categorical(["test","train","test","train"]),   | parmcards4;                              | 1 01/02/13 1 3 train foo  */
    /*  "F": "foo"                                              | exec(open('c:/oto/fn_python.py').read());| 1 01/02/13 1 3 test  foo  */
    /*  })                                                      | import pandas as pd                      | 1 01/02/13 1 3 train foo  */
    /*                                                          | import numpy as np                       |                           */
    /*                                                          |                                          --------------              */
    /*  <class 'pandas.core.frame.DataFrame'>                   | want = pd.DataFrame({                                  |             */
    /*  Index: 4 entries, 0 to 3                                | "A": 1.0,                                              |             */
    /*  Data columns (total 6 columns):                         | "B": pd.Timestamp("20130102"),                         |             */
    /*   #   Column  Non-Null Count  Dtype                      | "C": pd.Series(1,index=list(range(4)),dtype="float32"),|             */
    /*  ---  ------  --------------  -----                      | "D": np.array([3]*4,dtype="int32"),                    |             */
    /*   0   A       4 non-null      float64                    | "E": pd.Categorical(["test","train","test","train"]),  |             */
    /*   1   B       4 non-null      datetime64[s] (series)     | "F": "foo"                                             |             */
    /*   2   C       4 non-null      float32                    | })                                                     |             */
    /*   3   D       4 non-null      int32                      |                                                        |             */
    /*   4   E       4 non-null      category                   | print(want);                                           |             */
    /*   5   F       4 non-null      object                     | fn_tosas9x(want,outlib='d:/sd1/',outdsn='pywant');     |             */
    /*                                                          | ;;;;                                                   |             */
    /*   SOAPBOX ON                                             | %utl_pyendx;                                           |             */
    /*                                                          |                                                        |             */
    /*    Note all the datatypes, this                          |                                                        |             */
    /*    can cause all kinds of downstream problems?           | proc print data=sd1.pywant heading=vertical;           |             */
    /*                                                          | run;quit;                                              |             */
    /*   SOAPBOX OFF                                            |                                                        |             */
    /*                                                          |                                                        |             */
    /***********************************************************************************************************************************/

    /*              _
      ___ _ __   __| |
     / _ \ `_ \ / _` |
    |  __/ | | | (_| |
     \___|_| |_|\__,_|

    */
