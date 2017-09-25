
gui_simple.o:gui_simple.cpp
	g++ -c $^ -o $@ -I /usr/include/qt4 -I /usr/include/qt4/QtCore -I /usr/include/qt4/QtGui
GUISimple:gui_simple.o
	g++ $^ -o $@  -l QtCore -l QtGui

carre.o:carre.cpp
	g++ -c $^ -o $@ -I /usr/include/qt4 -I /usr/include/qt4/QtCore -I /usr/include/qt4/QtGui -I /net/cremi/costerta/espaces/travail/GeLog/qcustomplot
CourbeCarre:carre.o
	g++ $^ -o $@  -L /net/cremi/costerta/espaces/travail/GeLog/qcustomplot/sharedlib/compilation -l QtCore -l QtGui -l qcustomplot
	

#export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/net/cremi/costerta/espaces/travail/GeLog/qcustomplot/sharedlib/compilation/

