###########################

TransducerTechniquesSSIloadCellReader_ReubenPython3Class

Control class (including ability to hook to Tkinter GUI) to control/read load-cell data from the Transducer Techniques SSI.

https://www.transducertechniques.com/ssi.aspx

Reuben Brewer, Ph.D.

reuben.brewer@gmail.com

www.reubotics.com

Apache 2 License

Software Revision E, 05/10/2023

Verified working on: 

Python 3.8.

Windows 8.1, 10 64-bit

Raspberry Pi Buster 

(may work on Mac in non-GUI mode, but haven't tested yet)

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
CALd 5:  (specific to read/ersensor)
CAL 1nL:  (specific to reader)
CALPEr: 365
RR-1d: brd9-A
Loc 1: 1 0 0 1 1
Loc 2: 0 0 0 0
Loc 3: 0 0 0 0
Loc 4: 0 0 0 0 0

###########################

########################### Python module installation instructions, all OS's

test_program_for_TransducerTechniquesSSIloadCellReader_ReubenPython3Class_MultipleSensors.py, ListOfModuleDependencies: ['CSVdataLogger_ReubenPython3Class', 'MyPlotterPureTkinterStandAloneProcess_ReubenPython2and3Class', 'MyPrint_ReubenPython2and3Class', 'TransducerTechniquesSSIloadCellReader_ReubenPython3Class']

test_program_for_TransducerTechniquesSSIloadCellReader_ReubenPython3Class_MultipleSensors.py, ListOfModuleDependencies_TestProgram: []

test_program_for_TransducerTechniquesSSIloadCellReader_ReubenPython3Class_MultipleSensors.py, ListOfModuleDependencies_NestedLayers: ['ftd2xx', 'future.builtins', 'LowPassFilter_ReubenPython2and3Class', 'LowPassFilterForDictsOfLists_ReubenPython2and3Class', 'numpy', 'pexpect', 'psutil', 'serial', 'serial.tools']

test_program_for_TransducerTechniquesSSIloadCellReader_ReubenPython3Class_MultipleSensors.py, ListOfModuleDependencies_All:['CSVdataLogger_ReubenPython3Class', 'ftd2xx', 'future.builtins', 'LowPassFilter_ReubenPython2and3Class', 'LowPassFilterForDictsOfLists_ReubenPython2and3Class', 'MyPlotterPureTkinterStandAloneProcess_ReubenPython2and3Class', 'MyPrint_ReubenPython2and3Class', 'numpy', 'pexpect', 'psutil', 'serial', 'serial.tools', 'TransducerTechniquesSSIloadCellReader_ReubenPython3Class']

###########################

########################### FTDI installation instructions, Windows

(more to come)

###########################
