###########################

TransducerTechniquesSSIloadCellReader_ReubenPython3Class

Control class (including ability to hook to Tkinter GUI) to control/read load-cell data from the Transducer Techniques SSI.

https://www.transducertechniques.com/ssi.aspx

Reuben Brewer, Ph.D.

reuben.brewer@gmail.com

www.reubotics.com

Apache 2 License

Software Revision G, 11/19/2023

Verified working on:

Python 3.8.

Windows 8.1, 10, 11 64-bit

Raspberry Pi Buster

(may work on Mac in non-GUI mode, but haven't tested yet)

Note For test_program_for_TransducerTechniquesSSIloadCellReader_ReubenPython3Class_MultipleSensors.py:

1. The specific sensors that will be used (and, hence, the number of sensors) is set by the variable "TransducerTechniquesSSIloadCellReader_DevicesToReadSerialNumbersList".

2a. In Windows, you can get each sensor's USB-serial-device serial number by following the instructions in the USBserialDevice_GettingSerialNumberInWindows.png screenshot in this folder.

2b. IMPORTANT: Do NOT include the last "A" in the USB-serial-device serial number. For example, if the serial number from Device Manager is "AH02WWDYA", then only list "AH02WWDY" in "TransducerTechniquesSSIloadCellReader_DevicesToReadSerialNumbersList".

3. In Windows, you can manually set the latency timer for each sensor by following the instructions in the USBserialDevice_SettingLatencyTimerManuallyInWindows.png screenshot in this folder.

Note for ExcelPlot_CSVdataLogger_ReubenPython3Code__TransducerTechniquesSSIloadCellReader_MultipleSensors:

1. This file is currently configured for 3 sensors, plotting only their sum. These details can be changed in the function "CreateExcelChart".

###########################

###########################

Reader settings (consults SSI-Manual.pdf and SSI-SerialManual.pdf for more information):

SETuP: 0 _ _ 9

ConFG: 4 0 0 0 0

FiLtr: 1 1 1 0 0

dEC.Pt: d d d d d .

triG: 3 0

ALSEt: 1 1 0 4 0

tArE: 0 0 _ 0

SEr 1: 1 7 0

SEr 2: 0 0 1 _

SEr 3: 0 6

CALrt: (specific to calibration dates of reader and sensor)

LoG: 3 3 0 0 3

ALErt: 0 0 0 0

tirre: (specific to reader/sensor)

dAtE: (specific to user-ser date)

CALd 1: (specific to reader)

SErno: (specific to reader)

UnitS: 9 (specific to whatever units have been set on the LCD)

CALd 5:  (specific to reader/sensor)

CAL 1nL:  (specific to reader)

CALPEr: 365

RR-1d: brd9-A

Loc 1: 1 0 0 1 1

Loc 2: 0 0 0 0

Loc 3: 0 0 0 0

Loc 4: 0 0 0 0 0

###########################

########################### Python module installation instructions, all OS's

############

test_program_for_TransducerTechniquesSSIloadCellReader_ReubenPython3Class_MultipleSensors.py, ListOfModuleDependencies: ['CSVdataLogger_ReubenPython3Class', 'MyPlotterPureTkinterStandAloneProcess_ReubenPython2and3Class', 'MyPrint_ReubenPython2and3Class', 'TransducerTechniquesSSIloadCellReader_ReubenPython3Class']

test_program_for_TransducerTechniquesSSIloadCellReader_ReubenPython3Class_MultipleSensors.py, ListOfModuleDependencies_TestProgram: []

test_program_for_TransducerTechniquesSSIloadCellReader_ReubenPython3Class_MultipleSensors.py, ListOfModuleDependencies_NestedLayers: ['ftd2xx', 'future.builtins', 'LowPassFilter_ReubenPython2and3Class', 'LowPassFilterForDictsOfLists_ReubenPython2and3Class', 'numpy', 'pexpect', 'psutil', 'serial', 'serial.tools']

test_program_for_TransducerTechniquesSSIloadCellReader_ReubenPython3Class_MultipleSensors.py, ListOfModuleDependencies_All:['CSVdataLogger_ReubenPython3Class', 'ftd2xx', 'future.builtins', 'LowPassFilter_ReubenPython2and3Class', 'LowPassFilterForDictsOfLists_ReubenPython2and3Class', 'MyPlotterPureTkinterStandAloneProcess_ReubenPython2and3Class', 'MyPrint_ReubenPython2and3Class', 'numpy', 'pexpect', 'psutil', 'serial', 'serial.tools', 'TransducerTechniquesSSIloadCellReader_ReubenPython3Class']

For test_program_for_TransducerTechniquesSSIloadCellReader_ReubenPython3Class_MultipleSensors.py:

pip install psutil

pip install pyserial (NOT pip install serial).

pip install ftd2xx, ##https://pypi.org/project/ftd2xx/ #version 1.3.3 as of 11/08/23. For SetAllFTDIdevicesLatencyTimer function.

############

############

ExcelPlot_CSVdataLogger_ReubenPython3Code__TransducerTechniquesSSIloadCellReader_MultipleSensors.py, ListOfModuleDependencies: ['pandas', 'win32com.client', 'xlrd', 'xlsxwriter', 'xlutils.copy', 'xlwt']

ExcelPlot_CSVdataLogger_ReubenPython3Code__TransducerTechniquesSSIloadCellReader_MultipleSensors.py, ListOfModuleDependencies_TestProgram: []

ExcelPlot_CSVdataLogger_ReubenPython3Code__TransducerTechniquesSSIloadCellReader_MultipleSensors.py, ListOfModuleDependencies_NestedLayers: []

ExcelPlot_CSVdataLogger_ReubenPython3Code__TransducerTechniquesSSIloadCellReader_MultipleSensors.py, ListOfModuleDependencies_All:['pandas', 'win32com.client', 'xlrd', 'xlsxwriter', 'xlutils.copy', 'xlwt']

For ExcelPlot_CSVdataLogger_ReubenPython3Code__TransducerTechniquesSSIloadCellReader_MultipleSensors.py:

pip install pywin32         #version 305.1 11/8/23

pip install xlwt            #version 1.3.0 as of 11/8/23

pip install xlutils         #version 2.0.0 as of 11/8/23

pip install xlsxwriter      #version 3.1.9 as of 11/08/2023. Might have to manually delete older version from /lib/site-packages if it was distutils-managed. Works overall, but the function ".set_size" doesn't do anything.

############

###########################

########################### FTDI installation instructions, Windows

(more to come)

###########################
