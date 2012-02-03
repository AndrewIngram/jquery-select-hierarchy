jquery-select-hierarchy
=======================

Turns a single select box (note, doesn't support multiple select) with breadcrumb options into multiple dynamic ones to allow the hierarchy to be traversed. The original select is kept up-to-date with the choices so the form can be submitted as normal.

Sample Usage
------------

This example keeps the original select showing to illustrate the functionality::

  <!DOCTYPE html>
  <html>
  <body>
  
  <select class="drilldown">
    <option value="">------</option>
        <option value="1">Books</option>
        <option value="2">Books &gt; Fiction</option>
        <option value="3">Books &gt; Fiction &gt; Sci-Fi</option>
        <option value="4">Books &gt; Fiction &gt; Fantasy</option>
        <option value="5">Books &gt; Fiction &gt; Action</option>
        <option value="6">Books &gt; Fiction &gt; Romance</option>
        <option value="7">Books &gt; Travel</option>
        <option value="8">Books &gt; Travel &gt; Americas</option>
        <option value="9">Books &gt; Travel &gt; Europe</option>
        <option value="10">Books &gt; Travel &gt; Africa</option>
        <option value="11">Books &gt; Travel &gt; Australia</option>
        <option value="12">Books &gt; Biography</option>
        <option value="13">Games</option>
        <option value="14">Games &gt; X-Box 360</option>
        <option value="15">Games &gt; X-Box 360 &gt; Puzzle</option>
        <option value="16">Games &gt; X-Box 360 &gt; Roleplaying</option>
        <option value="17">Games &gt; X-Box 360 &gt; First-Person</option>
        <option value="18">Games &gt; Playstation 3</option>
        <option value="19">Games &gt; Playstation 3 &gt; Puzzle</option>
        <option value="20">Games &gt; Playstation 3 &gt; First-Person</option>
  <select>
  
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>
  <script src="../lib/js/jquery.select-hierarchy.js"></script>
  
  <script type="text/javascript">
    $('select.drilldown').selecthierarchy({ hideOriginal: false });
  </script>
  
  </body>
  </html>