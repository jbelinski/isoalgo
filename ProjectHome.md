<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-4069_thumb.png' title='IsoAlgo logo' height='70' width='134' alt='IsoAlgo logo' border='0'>

<h2>1. Introduction</h2>
IsoAlgo stands for piping Isometric drawing generation Algorithm. It can generate piping <br>isometric drawings in DXF format from PCF1. IsoAlgo reads the Piping Component File(PCF). <br>The PCF is a human readable text file containing physical and logical data on <br>each piping object in the pipeline.<br>
<br>
The Piping Component File(PCF) is the primary input for Personal ISOGEN®. PCFs are text <br>files containing component and routing information. For each component, they will <br>include various mandatory records to define the basic information of:<br>
<ul><li>Type - Flange, pipe, or valve, for example;<br>
</li><li>Coordinates and size of the end-points;<br>
</li><li>Shape(SKEY) to be used to represent the component on the isometric;<br>
PCFs are created by the piping design system extracting information from the piping <br>model. A single PCF can contain the data for a number of pipelines, but generally, <br>the piping design system extracts piping data for single pipeline only. Then Personal <br>ISOGEN will produce isometrics for one pipeline at a time.</li></ul>

The complex plant layouts and ship design result are drawings. Typically the design of<br>
<br>piping layouts requires the production of large amouts of isometric detail drawings. <br>The automatic generation of these isometric drawings will allow engineering staff to<br>
<br>concentrate on design activities therefore reducing the design cycle time span. <br>Nowdays many piping CAD software can layout piping in 3D and can generate Isometric <br>drawing automaticly, also can produce PCF intermidate file for data exchange.<br>
<br>
IsoAlgo gets piping data from PCF and generate isometric drawing in DXF format automatically.<br>
<br>
<h2>2. Usage</h2>
There are six files for IsoAlgo:<br>
<ul><li>IsoAlgo.dll<br>
</li><li>IsoAlgoTest.exe<br>
</li><li>IsoAlgoConfig.xml<br>
</li><li>IsoAlgoSymbolTemplate.xml<br>
</li><li>IsoAlgo User Guide.pdf<br>
</li><li>Run IsoAlgo.bat<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-28663_thumb.png' title='Files for IsoAlgo' height='405' width='554' alt='Figure 2.1 Files for IsoAlgo' border='0'></li></ul>

Figure 2.1 Files for IsoAlgo<br>
<br>
The usage of IsoAlgo is easy, only need edit the Run IsoAlgo.bat file, give the PCF file <br>name and the DXF file name, the content of the Run IsoAlgo.bat file is as follows:<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-16049_thumb.png' title='IsoAlgo Usage' height='161' width='465' alt='IsoAlgo Usage' border='0'>

Figure 2.2 IsoAlgo Usage<br>
<br>
When set the input PCF file name and the output DXF file name, then double click the <br>Run IsoAlgo.bat to run the IsoAlgo to generate the DXF file automatically.<br>
<br>
<h2>3. Configuration</h2>
Through the IsoAlgoConfig.xml file to configure the IsoAlgo, The IsoAlgoConfig.xml <br>content is as follow figure shown:<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-13800_thumb.png' title='IsoAlgoConfig.xml' height='542' width='554' alt='IsoAlgoConfig.xml' border='0'>

Figure 3.1 IsoAlgoConfig.xml<br>
<br>
There are many options to configure the IsoAlgo, mainly include the following:<br>
<ul><li>Sheet Layout Options;<br>
</li><li>Dimensioning Options;<br>
</li><li>Annotation Options;<br>
</li><li>Material List Options;<br>
</li><li>Material List Column Definitions;<br>
</li><li>Weld Numbering Options;</li></ul>

For example, if you want to change the paper size, you can modify the DrawingSize Name<br> to “A3”. Or you can change the ViewDirection to “NorthEast”. etc.<br>
<br>
<h2>4. Customize Symbol Template</h2>
IsoAlgo allows user to coutomize the symbol for some symbol keys by symbol template. <br>The symbol template is in the Cartesian coordinate system, as the following figure shows:<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-21891_thumb.png' title='Figure 4.1 Gate Valve Symbol Template' height='177' width='180' alt='Figure 4.1 Gate Valve Symbol Template' border='0'>

Figure 4.1 Gate Valve Symbol Template<br>
<br>
Then you can save the polylines for the symbol in IsoAlgoSymbolTemplate.xml file, <br>as following figure shows:<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-6303_thumb.png' title='Figure 4.2 Save Symbol Template Data ' height='472' width='554' alt='Figure 4.2 Save Symbol Template Data ' border='0'>

Figure 4.2 Save Symbol Template Data<br>
<br>
First, you should specicfy the Symbol Key(SKEY) for the symbol template;<br>
<br>
Then, give the arrive point and leave point for the symbol template;<br>
<br>
Finally, define the symbol graphics by polylines.<br>
<br>
<h2>5. Examples of Isometric Plots Generated by IsoAlgo</h2>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-5233_thumb.png' title='Figure 5.1 Piping model in AutoCAD Plant3D' height='434' width='364' alt='Figure 5.1 Piping model in AutoCAD Plant3D' border='0'>

Figure 5.1 Piping model in AutoCAD Plant3D<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-4282_thumb.png' title='Figure 5.2 Piping Isometric drawing generated by IsoAlgo' height='396' width='555' alt='Figure 5.2 Piping Isometric drawing generated by IsoAlgo' border='0'>

Figure 5.2 Piping Isometric drawing generated by IsoAlgo<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-20246_thumb.png' title='Figure 5.3 Piping Isometric drawing generated by IsoAlgo' height='398' width='556' alt='Figure 5.3 Piping Isometric drawing generated by IsoAlgo' border='0'>

Figure 5.3 Piping Isometric drawing generated by IsoAlgo<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-13069_thumb.png' title='Figure 5.4 Piping model in AutoCAD Plant3D' height='350' width='556' alt='Figure 5.4 Piping model in AutoCAD Plant3D' border='0'>

Figure 5.4 Piping model in AutoCAD Plant3D<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-16369_thumb.png' title='Figure 5.5 Piping Isometric drawing generated by IsoAlgo ' height='396' width='556' alt='Figure 5.5 Piping Isometric drawing generated by IsoAlgo ' border='0'>

Figure 5.5 Piping Isometric drawing generated by IsoAlgo<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-User-Guide_142E9/wps_clip_image-27927_thumb.png' title='Figure 5.6 Piping Isometric drawing generated by IsoAlgo' height='394' width='555' alt='Figure 5.6 Piping Isometric drawing generated by IsoAlgo' border='0'>

Figure 5.6 Piping Isometric drawing generated by IsoAlgo<br>
<br>
<h2>6.Feedback and Support</h2>
IsoAlgo is not finish yet, any feedback or suggestion is welcome, please send email to the author: <a href='mailto:IsoAlgo@gmail.com'>IsoAlgo@gmail.com</a>.<br>
<br>
For more information about IsoAlgo, please visit:<br>
<a href='http://www.cppblog.com/eryar/category/20555.html'>eryar IsoAlgo</a>