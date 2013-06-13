3-D-Category-Tag-Cloud-
=======================

3-D Category Tag Cloud for Opencart


1 .Place the below code in header.tpl just before </head> tag.


<script src="tag_cloud/jquery.tagcanvas.js" type="text/javascript"></script>
<script type="text/javascript">
      $(document).ready(function() {
        if(!$('#myCanvas').tagcanvas({
          textColour: '#CCC',
          outlineColour: '#CCC',
          reverse: true,
          depth: 1,
          maxSpeed: 0.05
        },'tags')) {
          // something went wrong, hide the canvas container
          $('#myCanvasContainer').hide();
        }
      });
    </script>
<!--------------  Tag Cloud	--------------->


2. Replace category.tpl file in Catalog->View->Theme->default->template->module->category.tpl with the file attached.



3. Refresh your browser and you have your tag cloud.

Ps : Since it uses HTML5 canvas element, it has issues with IE browsers below version 9.

  
Thanks

Roy M J
