# JS_SelectChildIndex
JavaScript / jQuery Select the child index and do something! 

```HTML
<!DOCTYPE html>
<html>
<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.4/jquery.min.js"></script>
<script>

  jQuery(() => {
     
    let parent = jQuery('#data_control').children();  

      // Show all child from this parent
      console.log( parent );
    
    parent.click(function() {

      //  Get which index or child being target !
      console.log( jQuery(this).index() );
      
      // Condition that index 2 must be selected and fireup* OR do something 
      2 == jQuery(this).index() && jQuery(this).css('color', 'red'); 

      /*
      0 <div class="data"> One </div>
      1 <div class="data"> two </div>
      2 <div class="data"> three </div>  This turns red
      3 <div class="data"> four </div>
      */

    });
  });

</script>
</head>
<body>

<div id="data_control">
 <div class="data"> One </div>
 <div class="data"> two </div>
 <div class="data"> three </div>
 <div class="data"> four </div>
</div>

</body>
</html>

```

<br /> Result : https://github.com/nielsoffice?tab=repositories | keyword : child
<br /> Related:
<br /> https://github.com/nielsoffice/JSGetChildArrayByKey
<br /> https://github.com/nielsoffice/SelectChildFromParentElement_jQuery
<br /> https://github.com/nielsoffice/JSGetParentsElemTraversing
