---
title: home
description: the home page
---

# GoldenGate Calculator  

<script>
  const scriptURL = 'https://script.google.com/macros/s/AKfycbzgb0tGoOzUElKU2nvC7XcTneymL1_sBaNGMDwJEG7jCMyPS0CzqU3tpb1CgfFpT-JOYA/exec'
  const form = document.forms['submit-to-google-sheet']
  ...
</script>
  
<form  name="submit-to-google-sheet">
   
    <input type="text" name="Product" placeholder="Assembly name" required>
    
	<input type="text" name="Description" placeholder="Brief description">
	
	<label for="Assembly_level">Assembly level</label>
	
	<select name="Assembly_level" id="Assembly_level">
 	 <option value="Level 0">Level 0</option>
  	 <option value="Level 1">Level 1</option>
 	 <option value="Level T">Level T</option>
 	 <option value="Custom">Custom</option>
	</select>
	
	
	<label for="Backbone">Acceptor:</label>
    <select name="Backbone" id="Backbone" onchange="yesnoCheck(this);" required>
 	 <option value="pICH41308">pICH41308 (CDS1)</option>
 	 <option value="pICH41331">pICH41331 (HRT)</option>
 	 <option value="pICH41295">pICH41295 (5U+Pro)</option>
 	 <option value="pICH41276">pICH41276 (3U+Ter)</option>
 	 <option value="pICH42012">pICH42012 (Cas12a gRNA)</option>
 	 <option value="pICH42009">pICH42009 (Cas9 gRNA)</option>
 	 <option value="pAGM1287">pAGM1287</option>
 	 <option value="pAGM1301">pAGM1301</option>
 	 <option value="L1P1">L1P1</option>
 	 <option value="L1P2">L1P2</option>
 	 <option value="L1P3">L1P3</option>
 	 <option value="L1P4">L1P4</option>
 	 <option value="L1P5">L1P5</option>
 	 <option value="L1P6">L1P6</option>
 	 <option value="L1P7">L1P7</option>
 	 <option value="pCAT.000">pCAT.000</option>
 	 <option value="pCAT.011">pCAT.011</option>
 	 <option value="pJMLT.000">pJMLT.000 </option>
 	 <option value="pJMLT.001">pJMLT.001 </option>
 	 <option value="pCAT.015">pJMLT.015 </option>
 	 <option value="pAGM4723">pAGM.4723 </option>
 	 <option value="pAGM8031">pAGM.8031 </option>
 	 <option value="Custom"></option>
	</select>	 
	
	
	<div id="ifYes" style="display: none;">
	<label for="Backbone_length">Backbone length (bp)</label>
    <input type="number" id="Backbone_length" name="Backbone_length" min="0" max="10000">
    </div>

    <label for="Backbone_stock">Backbone stock (ng/ul)</label>
    <input type="number" id="Backbone_stock" name="Backbone_stock" min="0" max="10000" >
    
    
	
  	<label for="backbone_ng">Backbone mass (ng)</label>
    <select name="backbone_ng" id="backbone_ng" required>
 	 <option value="50">50</option>
  	 <option value="75">75</option>
 	 <option value="100">100</option>
 	 <option value="Custom"></option>
	</select>	 
	   	
    <input type="text" name="Insert1_name" placeholder="Insert 1 name" required>
    
    <label for="Insert1_length">Length (bp)</label>
    <input type="number" value="0" id="Insert1_length" name="Insert1_length" min="0" max="10000">
    
    <label for="Insert1_stock">Stock (ng/ul)</label>
    <input type="number" value="0" id="Insert1_stock" name="Insert1_stock" min="0" max="10000" >
    
  	<input type="text" name="Description1" value="Description 1">

	
    <input type="text" name="Insert2_name" value ="Insert2 name" >
 
  	<label for="Insert2_length">Length (bp)</label>
    <input type="number" value="0" id="Insert2_length" name="Insert2_length" min="0" max="10000" >
    <label for="Insert1_stock">Stock (ng/ul)</label>
    <input type="number" value="0" id="Insert1_stock" name="Insert1_stock" min="0" max="10000" >
    
  	<input type="text" value ="Description 2" name="Description2">

	
	<input type="text" name="Insert3_name" value ="Insert3 name" >
	
 	<label for="Insert3_length">Length (bp)</label>
    <input type="number" value="0" id="Insert3_length" name="Insert3_length" min="0" max="10000" >
    
    <label for="Insert3_stock">Stock (ng/ul)</label>
    <input type="number" value="0" id="Insert3_stock" name="Insert3_stock" min="0" max="10000">
    
    <input type="text" name="Description3" value ="Description 3" >

	
	
	<input type="text" name="Insert4_name" value ="Insert4 name" >
	
    <label for="Insert4_length">Length (bp)</label>
    <input type="number" value="0"  id="Insert4_length" name="Insert4_length" min="0" max="10000">
    
    <label for="Insert4_stock">Stock (ng/ul)</label>
    <input type="number" value="0" id="Insert4_stock" name="Insert4_stock" min="0" max="10000">
    
    <input type="text" name="Description4" value ="Description 4" >

	
	
	<input type="text" name="Insert5_name" value="Insert5 Name">
	
    <label for="Insert5_length">Length (bp)</label>
    <input type="number" value="0" id="Insert5_length" name="Insert5_length" min="0" max="10000" >
    
    <label for="Insert5_stock">Stock (ng/ul)</label>
    <input type="number" value="0"  id="Insert5_stock" name="Insert5_stock" min="0" max="10000">
    
  	<input type="text" name="Description5" value ="Description 5" >

	
	<input type="text" name="Insert6_name" value ="Insert6 name" >
	
   	<label for="Insert6_length">Length (bp)</label>
    <input type="number" value="0" id="Insert6_length" name="Insert6_length" min="0" max="10000">
    
    <label for="Insert6_stock">Stock (ng/ul)</label>
    <input type="number" value="0"  id="Insert6_stock" name="Insert6_stock" min="0" max="10000">
    
  	<input type="text" name="Description6" value ="Description 6" >

	<input type="text" name="Insert7_name" value ="Insert7 name" >
	
    <label for="Insert7_length">Length (bp)</label>
    <input type="number" value="0" id="Insert7_length" name="Insert7_length" min="0" max="10000">
    
    <label for="Insert7_stock">Stock (ng/ul)</label>
    <input type="number" value="0" id="Insert7_stock" name="Insert67stock" min="0" max="10000">
    
    <input type="text" name="Description7" value ="Description 7" >


	<button onclick="window.location.href='https://cakelabdna.github.io/2768cd316e26196a473a415dc9bdb2c707f1dbd4/results.html'">ASSEMBLE</button>

</form>  

# Output

# [Assembly Report](https://docs.google.com/spreadsheets/d/12G5TwARG7o5OzgPICj9YPiSczuWmx1yngZYTKdHQzaY/edit#gid=683324272&range=A1:J15)    
<iframe width="1000" height="480" src="https://docs.google.com/spreadsheets/d/12G5TwARG7o5OzgPICj9YPiSczuWmx1yngZYTKdHQzaY/htmlembed/sheet?gid=683324272&range=A1:J15"></iframe>

# [Assembly Queue](https://docs.google.com/spreadsheets/d/12G5TwARG7o5OzgPICj9YPiSczuWmx1yngZYTKdHQzaY/edit#gid=2110853524)    
<iframe width="1000" height="500" src="https://docs.google.com/spreadsheets/d/12G5TwARG7o5OzgPICj9YPiSczuWmx1yngZYTKdHQzaY/htmlembed/sheet?gid=2110853524&range=A1:CA20"></iframe>

# Validate Assembly History by DNA Sequencing
<iframe width="1000" height="600" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRGrSl_Dh8BnqAPCtToCj-RWnE3h5z8GubHpB_kGyVxtgLD7cYqmFJc3aYs80663PxQmnjvR2DbF39x/pubhtml?gid=0&amp;single=true&amp;AllowTyping=True;widget=false&amp;headers=false"></iframe>

# User-specific DNA libraries
## AS
### ASGate Level 0
<iframe width="1000" height="400" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='L0%20Parts'!A1%3AO16&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>
### ASGate Level 1
<iframe width="1000" height="454" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='L1%20Parts'!A1%3AN20&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>
### ASGate Level T
<iframe width="1000" height="310" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='LT%20Parts'!A1%3AN13&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>

## DGK
### DGK0
### DGK1
### DGKM

## JML
### JML0
### JML1
### JMLT

## XX
### XX0
### XX1
### XXT


<script>
  const scriptURL = 'https://script.google.com/macros/s/AKfycbzgb0tGoOzUElKU2nvC7XcTneymL1_sBaNGMDwJEG7jCMyPS0CzqU3tpb1CgfFpT-JOYA/exec'
  const form = document.forms['submit-to-google-sheet']

  form.addEventListener('submit', e => {
    e.preventDefault()
    fetch(scriptURL, { method: 'POST', body: new FormData(form)})
      .then(response => console.log('Success!', response))
      .catch(error => console.error('Error!', error.message))
  })
  
   function showLoadingIndicator () {
      form.classList.add('is-hidden')
      loading.classList.remove('is-hidden')
    }

    function showSuccessMessage (response) {
      console.log('Success!', response)
      setTimeout(() => {
        successMessage.classList.remove('is-hidden')
        loading.classList.add('is-hidden')
      }, 500)
    }

    function showErrorMessage (error) {
      console.error('Error!', error.message)
      setTimeout(() => {
        errorMessage.classList.remove('is-hidden')
        loading.classList.add('is-hidden')
      }, 500)
    }
</script>

<script type="text/javascript">
 	function yesnoCheck(that) {
  	  if (that.value == "Custom") {
  		alert("check");
        document.getElementById("ifYes").style.display = "block";
    	} else {
        document.getElementById("ifYes").style.display = "none";
   		 }
		}
</script>

<script src="http://code.jquery.com/jquery-1.4.2.min.js"></script> <script> var x = document.getElementsByClassName("site-footer-credits"); setTimeout(() => { x[0].remove(); }, 10); </script>



