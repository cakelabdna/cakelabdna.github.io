---
title: home
description: the home page
---

# CyanoGate Calculator  

<form id="test-form">
  
  <div>
    <label>Product</label>
    <input type="text" name="Product" placeholder="Field 1"/>
  </div>

  <div>
    <label>Insert 1</label>
    <input type="text" name="Insert 1" placeholder="Field 2"/>
  </div>
  
  <div>
    <label>Insert 2</label>
    <input type="text" name="Insert 2" placeholder="Field 3"/>
  </div>
  
  <div>
    <label>Insert 3</label>
    <input type="text" name="Insert 3" placeholder="Field 4"/>
  </div>
  
  <div>
    <label>Insert 4</label>
    <input type="text" name="Insert 4" placeholder="Field 4"/>
  </div>
  
<div>
    <label>Insert 5</label>
    <input type="text" name="Insert 5" placeholder="Field 4"/>
  </div>

<div>
    <label>Insert 6</label>
    <input type="text" name="Insert 6" placeholder="Field 4"/>
  </div>

<div>
    <label>Insert 7</label>
    <input type="text" name="Insert 7" placeholder="Field 4"/>
  </div>


  <div>
    <button type="submit"id="submit-form">Submit</button>
  </div>
  
var $form = $('form#test-form'),
    url = 'https://script.google.com/macros/s/AKfycbxA30Ow8WCUq3pf0i8m3Qa8R0MNxkDYO5WnHnzkLBL9PiwXJt1E1JqZNA/exec'

$('#submit-form').on('click', function(e) {
  e.preventDefault();
  var jqxhr = $.ajax({
    url: url,
    method: "GET",
    dataType: "json",
    data: $form.serializeObject()
  }).success(
    // do something
  );
})

</form>




<iframe width="1000" height="450" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='AssemblyCalculator'!A1%3AK14&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>

# Assembly History
<iframe width="1000" height="400" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRGrSl_Dh8BnqAPCtToCj-RWnE3h5z8GubHpB_kGyVxtgLD7cYqmFJc3aYs80663PxQmnjvR2DbF39x/pubhtml?gid=0&amp;single=true&amp;AllowTyping=True;widget=true&amp;headers=false"></iframe>

## ASGate Level 0
<iframe width="1000" height="400" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='L0%20Parts'!A1%3AO16&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>

## ASGate Level 1
<iframe width="1000" height="454" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='L1%20Parts'!A1%3AN20&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>

## ASGate Level T
<iframe width="1000" height="310" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='LT%20Parts'!A1%3AN13&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>


<script src="http://code.jquery.com/jquery-1.4.2.min.js"></script> <script> var x = document.getElementsByClassName("site-footer-credits"); setTimeout(() => { x[0].remove(); }, 10); </script>



