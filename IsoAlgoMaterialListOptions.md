# 1. Introduction #
IsoAlgo can produce a customised Material List. The Material List columns maybe selected from one attribute of the component.

# 2. Material List Options #
You can specify the material list datum position on the drawing. The entries in the material list are numbered sequentially, each entry contains the material’s description, nominal size, item code and quantity. You can customize the material list by modify the IsoAlgoConfig.xml:
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-Material-List-Options_11864/wps_clip_image-6813_thumb.png' title='Figure 1 Material List Options in IsoAlgoConfig.xml ' height='364' width='533' alt='Figure 1 Material List Options in IsoAlgoConfig.xml ' border='0' /> <br>
Figure 1 Material List Options in IsoAlgoConfig.xml<br>
<br>
First, you specify the character size and the line spacing percent of the material list;<br>
Second, specify the material list datum position on the drawing, modify the X and Y value for the ListDatum. The IsAscending is used to control the material list direction. If the IsAscending is true, the material list ‘s part number from 1 to N is from up to the bottom, else the material list’s part number from 1 to N is from bottom to the up.<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-Material-List-Options_11864/wps_clip_image-1402_thumb.png' title='Figure 2 Material List with IsAscending is true' height='263' width='556' alt='Figure 2 Material List with IsAscending is true' border='0' /> <br>
Figure 2 Material List with IsAscending is true<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-Material-List-Options_11864/wps_clip_image-22754_thumb.png' title='Figure 3 Material List with IsAscending is false ' height='236' width='556' alt='Figure 3 Material List with IsAscending is false ' border='0' /> <br>
Figure 3 Material List with IsAscending is false<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-Material-List-Options_11864/wps_clip_image-25567_thumb.png' title='Figure 4 Isometric drawing with Material List' height='394' width='554' alt='Figure 4 Isometric drawing with Material List' border='0' /> <br>
Figure 4 Isometric drawing with Material List<br>
<br>
<br>
<h1>3. Material List Column Definitions</h1>
You can specify each column of the material list, the import attribute is Fill and Width. The Fill is used to map the value for the material list and the Width is used to set the width of that column. So you can decide the content of each column. For example, if you do not want the ITEMCODE column, you can remove that column.<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-Material-List-Options_11864/wps_clip_image-12218_thumb.png' title='Figure 5 Material List Column Definitions ' height='276' width='554' alt='Figure 5 Material List Column Definitions ' border='0' /> <br>
Figure 5 Material List Column Definitions<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-Material-List-Options_11864/wps_clip_image-20577_thumb.png' title='Figure 6 Material List Column Definitions Result' height='267' width='556' alt='Figure 6 Material List Column Definitions Result' border='0' /> <br>
Figure 6 Material List Column Definitions Result<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-Material-List-Options_11864/image_thumb.png' title='Isometric drawing generatd by IsoAlgo' height='684' width='963' alt='Isometric drawing generatd by IsoAlgo' border='0' /> <br>
Figure 7 Isometric drawing generatd by IsoAlgo<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-Material-List-Options_11864/image_thumb_1.png' title='Isometric drawing generatd by IsoAlgo' height='685' width='964' alt='Isometric drawing generatd by IsoAlgo' border='0' /> <br>
Figure 8 Isometric drawing generatd by IsoAlgo<br>
<br>
<img src='http://www.cppblog.com/images/cppblog_com/eryar/Windows-Live-Writer/IsoAlgo-Material-List-Options_11864/image_thumb_2.png' title='Isometric drawing generatd by IsoAlgo' height='682' width='963' alt='Isometric drawing generatd by IsoAlgo' border='0' />
Figure 9 Isometric drawing generatd by IsoAlgo