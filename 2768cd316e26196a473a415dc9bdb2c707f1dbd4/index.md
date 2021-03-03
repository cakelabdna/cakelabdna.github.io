---
title: home
description: the home page
---

# CyanoGate Calculator  

<script src="https://wzrd.in/standalone/formdata-polyfill"></script>
<script src="https://wzrd.in/standalone/promise-polyfill@latest"></script>
<script src="https://wzrd.in/standalone/whatwg-fetch@latest"></script>

<script>
  const scriptURL = 'https://cakelabdna.github.io/2768cd316e26196a473a415dc9bdb2c707f1dbd4/index.html'
  const form = document.forms['submit-to-google-sheet']
  ...
</script>

  
<form  name="submit-to-google-sheet" action="https://cakelabdna.github.io/2768cd316e26196a473a415dc9bdb2c707f1dbd4/index.html">
   
    <input type="text" name="Product" placeholder="Assembly name" required>
	<input type="text" name="Description" placeholder="Brief description" required>
	<label for="Assembly_level">Assembly level</label>
	<select name="Assembly_level" id="Assembly_level">
 	 <option value="Level 0">Level 0</option>
  	 <option value="Level 1">Level 1</option>
 	 <option value="Level T">Level T</option>
 	 <option value="Custom">Custom</option>
	</select>
    <label for="inserts">Number of inserts:</label>
    <input type="number" id="inserts" name="inserts" min="1" max="7">
	<input type="text" name="Backbone" placeholder="Backbone Acceptor" required>	
	<input type="text" name="Backbone_length" placeholder="Backbone Length (bp)" required>
	<input type="text" name="Backbone_stock" placeholder="Backbone [Stock] (ng/ul)" required>	
  	<input type="text" name="backbone_ng" placeholder="Backbone mass" required>
    <input type="text" name="Insert1_name" placeholder="Insert 1 Name" required>
    <input type="text" name="Insert1_length" placeholder="Insert 1 Length" required>
    <input type="text" name="Insert1_stock" placeholder="Insert 1 Stock (ng/ul)" required>
    <input type="text" name="Insert1_ratio" placeholder="I:B Ratio" required>
    <input type="text" name="Insert2_name" placeholder="Insert 2 Name">
    <input type="text" name="Insert2_length" placeholder="Insert 2 Length">
    <input type="text" name="Insert2_stock" placeholder="Insert 2 Stock (ng/ul)"> 
    <input type="text" name="Insert2_ratio" placeholder="I:B Ratio">
    <input type="text" name="Insert3_name" placeholder="Insert 3 Name">
    <input type="text" name="Insert3_length" placeholder="Insert 3 Length">
    <input type="text" name="Insert3_stock" placeholder="Insert 3 Stock (ng/ul)">
    <input type="text" name="Insert3_ratio" placeholder="I:B Ratio">
    <input type="text" name="Insert4_name" placeholder="Insert 4 Name">
    <input type="text" name="Insert4_length" placeholder="Insert 4 Length">
    <input type="text" name="Insert4_stock" placeholder="Insert 4 Stock (ng/ul)">
    <input type="text" name="Insert4_ratio" placeholder="I:B Ratio"> 
    <input type="text" name="Insert5_name" placeholder="Insert 5 Name">
    <input type="text" name="Insert5_length" placeholder="Insert 5 Length">
    <input type="text" name="Insert5_stock" placeholder="Insert 5 Stock (ng/ul)">
    <input type="text" name="Insert5_ratio" placeholder="Insert 5 I:B Ratio">
    <input type="text" name="Insert6_name" placeholder="Insert 6 Name">
    <input type="text" name="Insert6_length" placeholder="Insert 6 Length">
    <input type="text" name="Insert6_stock" placeholder="Insert 6 Stock (ng/ul)">
    <input type="text" name="Insert6_ratio" placeholder="Insert 6 I:B Ratio">
    <input type="text" name="Insert7_name" placeholder="Insert 7 Name">
    <input type="text" name="Insert7_length" placeholder="Insert 7 Length">
    <input type="text" name="Insert7_stock" placeholder="Insert 7 Stock (ng/ul)">
    <input type="text" name="Insert7_ratio" placeholder="Insert 7 I:B Ratio">
  	<button type="submit">ASSEMBLE</button> 
    
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


  
# Assembly Details
<iframe width="1000" height="420" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTWhc3ZkTQasnqLvXL5ais9haD2w1RxJI_au9acA11FKOAKb9akM6gWdu29c85KLnt63rr903oUpDlk/pubhtml?gid=683324272&amp;single=true&amp;widget=true&amp;headers=false"></iframe>
# Assembly History
<iframe width="1000" height="600" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRGrSl_Dh8BnqAPCtToCj-RWnE3h5z8GubHpB_kGyVxtgLD7cYqmFJc3aYs80663PxQmnjvR2DbF39x/pubhtml?gid=0&amp;single=true&amp;AllowTyping=True;widget=true&amp;headers=false"></iframe>

## ASGate Level 0
<iframe width="1000" height="400" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='L0%20Parts'!A1%3AO16&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>

## ASGate Level 1
<iframe width="1000" height="454" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='L1%20Parts'!A1%3AN20&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>

## ASGate Level T
<iframe width="1000" height="310" frameborder="0" scrolling="no" src="https://universityofcambridgecloud-my.sharepoint.com/personal/as2945_cam_ac_uk/_layouts/15/Doc.aspx?sourcedoc={1f4b5bc8-4e9e-4ea3-87ff-2c1e991b61fe}&action=embedview&AllowTyping=True&Item='LT%20Parts'!A1%3AN13&wdHideGridlines=True&wdDownloadButton=True&wdInConfigurator=True"></iframe>


<script src="http://code.jquery.com/jquery-1.4.2.min.js"></script> <script> var x = document.getElementsByClassName("site-footer-credits"); setTimeout(() => { x[0].remove(); }, 10); </script>



