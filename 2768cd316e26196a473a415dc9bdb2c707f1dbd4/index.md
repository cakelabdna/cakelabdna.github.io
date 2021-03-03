---
title: home
description: the home page
---

# CyanoGate Calculator  

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
	
    <label for="inserts">Number of inserts:</label>
    <input type="number" id="inserts" name="inserts" min="1" max="7">
    
	<input type="text" name="Backbone" placeholder="Backbone Acceptor" >	
	
	<input type="text" name="Backbone_length" placeholder="Backbone Length (bp)" >
	
	<input type="text" name="Backbone_stock" placeholder="Backbone [Stock] (ng/ul)" >	
	
  	<label for="backbone_ng">Backbone mass (ng)</label>
    <select name="backbone_ng" id="backbone_ng" required>
 	 <option value="50">50</option>
  	 <option value="75">75</option>
 	 <option value="100">100</option>
 	 <option value="Custom"></option>
	</select>	 
	   	
    <input type="text" name="Insert1_name" placeholder="Insert 1 Name" >
    
    <label for="Insert1_length">Insert 1 Length (bp)</label>
    <input type="number" id="Insert1_length" name="Insert1_length" min="0" max="10000">
    
    <label for="Insert1_stock">Insert 1 Stock (ng/ul)</label>
    <input type="number" id="Insert1_stock" name="Insert1_stock" min="0" max="10000" >
    
    <label for="Insert1_ratio">I1/B Ratio</label>
    <select name="Insert1_ratio" id="Insert1_ratio">
 	 <option value="2">2</option>
  	 <option value="10">10</option>
 	 <option value="20">20</option>
 	 <option value="Custom"></option>
	</select>	
	
    <input type="text" name="Insert2_name" placeholder="Insert 2 Name">
 
  	<label for="Insert2_length">Insert 2 Length (bp)</label>
    <input type="number" id="Insert2_length" name="Insert2_length" min="0" max="10000" >
    <label for="Insert1_stock">Insert 1 Stock (ng/ul)</label>
    <input type="number" id="Insert1_stock" name="Insert1_stock" min="0" max="10000" >
    
    <label for="Insert2_ratio">I2/B Ratio</label>
    <select name="Insert2_ratio" id="Insert2_ratio">
 	 <option value="2">2</option>
  	 <option value="10">10</option>
 	 <option value="20">20</option>
 	 <option value="Custom"></option>
	</select>	    
	
	<input type="text" name="Insert3_name" placeholder="Insert 3 Name">
	
 	<label for="Insert3_length">Insert 3 Length (bp)</label>
    <input type="number" id="Insert3_length" name="Insert3_length" min="0" max="10000" >
    
    <label for="Insert3_stock">Insert 3 Stock (ng/ul)</label>
    <input type="number" id="Insert3_stock" name="Insert3_stock" min="0" max="10000">
    
    <label for="Insert3_ratio">I3/B Ratio</label>
    <select name="Insert3_ratio" id="Insert3_ratio">
 	 <option value="2">2</option>
  	 <option value="10">10</option>
 	 <option value="20">20</option>
 	 <option value="Custom"></option>
	</select>	    
	
	
	<input type="text" name="Insert4_name" placeholder="Insert 4 Name">
	
    <label for="Insert4_length">Insert 4 Length (bp)</label>
    <input type="number" id="Insert4_length" name="Insert4_length" min="0" max="10000">
    
    <label for="Insert4_stock">Insert 4 Stock (ng/ul)</label>
    <input type="number" id="Insert4_stock" name="Insert4_stock" min="0" max="10000">
    
    <label for="Insert4_ratio">I4/B Ratio</label>
    <select name="Insert4_ratio" id="Insert4_ratio">
 	 <option value="2">2</option>
  	 <option value="10">10</option>
 	 <option value="20">20</option>
 	 <option value="Custom"></option>
	</select>	
	
	
	
	
	<input type="text" name="Insert5_name" placeholder="Insert 5 Name">
	
    <label for="Insert5_length">Insert 5 Length (bp)</label>
    <input type="number" id="Insert5_length" name="Insert5_length" min="0" max="10000" >
    
    <label for="Insert5_stock">Insert 5 Stock (ng/ul)</label>
    <input type="number" id="Insert5_stock" name="Insert5_stock" min="0" max="10000">
    
    <label for="Insert5_ratio">I5/B Ratio</label>
    <select name="Insert5_ratio" id="Insert5_ratio">
 	 <option value="2">2</option>
  	 <option value="10">10</option>
 	 <option value="20">20</option>
 	 <option value="Custom"></option>
	</select>	
	
	
	
	<input type="text" name="Insert6_name" placeholder="Insert 6 Name">
	
   	<label for="Insert6_length">Insert 6 Length (bp)</label>
    <input type="number" id="Insert6_length" name="Insert6_length" min="0" max="10000">
    
    <label for="Insert6_stock">Insert 6 Stock (ng/ul)</label>
    <input type="number" id="Insert6_stock" name="Insert6_stock" min="0" max="10000">
    
    <label for="Insert6_ratio">I6/B Ratio</label>
    <select name="Insert6_ratio" id="Insert6_ratio">
 	 <option value="2">2</option>
  	 <option value="10">10</option>
 	 <option value="20">20</option>
 	 <option value="Custom"></option>
	</select>	
	
	
	
	
	
	<input type="text" name="Insert7_name" placeholder="Insert 7 Name">
	
    <label for="Insert7_length">Insert 7 Length (bp)</label>
    <input type="number" id="Insert7_length" name="Insert7_length" min="0" max="10000">
    
    <label for="Insert7_stock">Insert 7 Stock (ng/ul)</label>
    <input type="number" id="Insert7_stock" name="Insert67stock" min="0" max="10000">
    
    <label for="Insert7_ratio">I7/B Ratio</label>
    <select name="Insert7_ratio" id="Insert7_ratio">
 	 <option value="2">2</option>
  	 <option value="10">10</option>
 	 <option value="20">20</option>
 	 <option value="Custom"></option>
	</select>	    
    <button type="submit" onClick="window.location.href=window.location.href">Submit and Refresh</button>

</form>  





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


  
# Assembly Report
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTWhc3ZkTQasnqLvXL5ais9haD2w1RxJI_au9acA11FKOAKb9akM6gWdu29c85KLnt63rr903oUpDlk/pubhtml?widget=true&amp;headers=false"></iframe>

# Assembly History
<iframe width="1000" height="600" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRGrSl_Dh8BnqAPCtToCj-RWnE3h5z8GubHpB_kGyVxtgLD7cYqmFJc3aYs80663PxQmnjvR2DbF39x/pubhtml?gid=0&amp;single=true&amp;AllowTyping=True;widget=true&amp;headers=false"></iframe>

## ASGate Level 0
<iframe width="1000" height="400" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='L0%20Parts'!A1%3AO16&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>

## ASGate Level 1
<iframe width="1000" height="454" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='L1%20Parts'!A1%3AN20&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>

## ASGate Level T
<iframe width="1000" height="310" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='LT%20Parts'!A1%3AN13&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>


<script src="http://code.jquery.com/jquery-1.4.2.min.js"></script> <script> var x = document.getElementsByClassName("site-footer-credits"); setTimeout(() => { x[0].remove(); }, 10); </script>



