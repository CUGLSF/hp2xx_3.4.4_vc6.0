# <center>hp2xx_3.4.4_vc6.0</center>

##Introduction
This project is mainly based on the open source project [hp2xx](http://gnuwin32.sourceforge.net/packages/hp2xx.htm)(A HPGL converter into some vector- and raster formats).

## My interests of hp2xx
Here,I mainly focus on the function that **hp2xx can interpret the HPGL files to 
CNC *.nc files.**

## Compile
I compiled hp2xx on my **Windows 10 system** using the **Microsoft Visual C++ 6.0** compiler(a very small utility although it is outdated.)

## How to convert a HPGL file to NC file
Execute the program with the parameters: **-m nc -f dt.nc dt.plt**(Assuming the input HPGL file is "dt.plt")

The simple explanation of above options:

“**--mode (-m) string**”
	
	After the '-m' option follows the detailed mode(such as **dxt**,**cad**,etc).We want to get a *.nc file and we specify the mode to "**nc**".
 
"**--outfile (-f) string**"

	Name of output file. If omitted, hp2xx generates the name from the input file name and the current mode string. `-f-' causes hp2xx to write to stdout. Default: none.

If you want to know more about the options of hp2xx,please go here:[**hp2xx general options**](http://www.delorie.com/gnu/docs/hp2xx/hp2xxinf_31.html)

If you specify the parameters in the compiler.The screenshot following shows the detailed configuration:

![](http://i.imgur.com/CTadDXy.png)

After execute the hp2xx.exe with the above parameters,you can get the CNC ***.nc** file with the same name of the original ***plt** file.


