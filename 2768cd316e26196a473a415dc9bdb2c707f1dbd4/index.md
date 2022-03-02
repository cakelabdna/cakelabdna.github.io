---
title: CyanoGate 2.0
description: An expanded MoClo Toolbox for Synthetic Biology in Cyanobacteria
---

# Assembly Calculator  

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
	
	
	<label for="inserts">How many inserts?</label>
    <input type="number" id="inserts" name="inserts" min="1" max="7" >
    
	
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
 	 <option value="Custom">Custom</option>
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

	
    <input type="text" name="Insert2_name" value ="" >
 
  	<label for="Insert2_length">Length (bp)</label>
    <input type="number" value="0" id="Insert2_length" name="Insert2_length" min="0" max="10000" >
    <label for="Insert2_stock">Stock (ng/ul)</label>
    <input type="number" value="0" id="Insert2_stock" name="Insert2_stock" min="0" max="10000" >
    
  	<input type="text" value ="Description 2" name="">

	
	<input type="text" name="Insert3_name" value ="" >
	
 	<label for="Insert3_length">Length (bp)</label>
    <input type="number" value="0" id="Insert3_length" name="Insert3_length" min="0" max="10000" >
    
    <label for="Insert3_stock">Stock (ng/ul)</label>
    <input type="number" value="0" id="Insert3_stock" name="Insert3_stock" min="0" max="10000">
    
    <input type="text" name="Description3" value ="" >

	
	
	<input type="text" name="Insert4_name" value ="" >
	
    <label for="Insert4_length">Length (bp)</label>
    <input type="number" value="0"  id="Insert4_length" name="Insert4_length" min="0" max="10000">
    
    <label for="Insert4_stock">Stock (ng/ul)</label>
    <input type="number" value="0" id="Insert4_stock" name="Insert4_stock" min="0" max="10000">
    
    <input type="text" name="Description4" value ="" >

	
	
	<input type="text" name="Insert5_name" value="">
	
    <label for="Insert5_length">Length (bp)</label>
    <input type="number" value="0" id="Insert5_length" name="Insert5_length" min="0" max="10000" >
    
    <label for="Insert5_stock">Stock (ng/ul)</label>
    <input type="number" value="0"  id="Insert5_stock" name="Insert5_stock" min="0" max="10000">
    
  	<input type="text" name="Description5" value ="" >

	
	<input type="text" name="Insert6_name" value ="" >
	
   	<label for="Insert6_length">Length (bp)</label>
    <input type="number" value="0" id="Insert6_length" name="Insert6_length" min="0" max="10000">
    
    <label for="Insert6_stock">Stock (ng/ul)</label>
    <input type="number" value="0"  id="Insert6_stock" name="Insert6_stock" min="0" max="10000">
    
  	<input type="text" name="Description6" value ="" >

	<input type="text" name="Insert7_name" value ="" >
	
    <label for="Insert7_length">Length (bp)</label>
    <input type="number" value="0" id="Insert7_length" name="Insert7_length" min="0" max="10000">
    
    <label for="Insert7_stock">Stock (ng/ul)</label>
    <input type="number" value="0" id="Insert7_stock" name="Insert67stock" min="0" max="10000">
    
    <input type="text" name="Description7" value ="" >


	<button onclick="window.location.href='https://cakelabdna.github.io/2768cd316e26196a473a415dc9bdb2c707f1dbd4/results.html'">ASSEMBLE</button>

</form>  

# Output

# [Assembly Report](https://docs.google.com/spreadsheets/d/12G5TwARG7o5OzgPICj9YPiSczuWmx1yngZYTKdHQzaY/edit#gid=683324272&range=A1:J15)    
<iframe width="1000" height="480" src="https://docs.google.com/spreadsheets/d/12G5TwARG7o5OzgPICj9YPiSczuWmx1yngZYTKdHQzaY/htmlembed/sheet?gid=683324272&range=A1:J15"></iframe>

# Table of New Acceptors
<table>
<thead>
  <tr>
    <th>Tube Number</th>
    <th>MoClo</th>
    <th>pJML</th>
    <th>Insert</th>
    <th>Successful Assembly</th>
    <th>Succesful sequencing</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>1</td>
    <td>PICH41233</td>
    <td>pJMLA0.001</td>
    <td>Pro</td>
    <td>y</td>
    <td>m</td>
  </tr>
  <tr>
    <td>2</td>
    <td>PAGM1251</td>
    <td>pJMLA0.002</td>
    <td>Pro+5U(f)</td>
    <td>y</td>
    <td>m</td>
  </tr>
  <tr>
    <td>3</td>
    <td>PICH41295</td>
    <td>pJMLA0.003</td>
    <td>Pro+5U</td>
    <td>y</td>
    <td>m</td>
  </tr>
  <tr>
    <td>4</td>
    <td>PAGM1263</td>
    <td>pJMLA0.004</td>
    <td>5U(f)</td>
    <td>y</td>
    <td>m</td>
  </tr>
  <tr>
    <td>5</td>
    <td>PICH41246</td>
    <td>pJMLA0.005</td>
    <td>5U</td>
    <td>y</td>
    <td>y</td>
  </tr>
  <tr>
    <td>6</td>
    <td>PAGM1276</td>
    <td>pJMLA0.006</td>
    <td>NT1</td>
    <td>y</td>
    <td>y</td>
  </tr>
  <tr>
    <td>7</td>
    <td>PICH41258</td>
    <td>pJMLA0.007</td>
    <td>SP</td>
    <td>y</td>
    <td>m</td>
  </tr>
  <tr>
    <td>8</td>
    <td>PICH41308</td>
    <td>pJMLA0.008</td>
    <td>CDS1</td>
    <td>y</td>
    <td>y</td>
  </tr>
  <tr>
    <td>9</td>
    <td>PICH41287</td>
    <td>pJMLA0.009</td>
    <td>CDS1 ns</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>10</td>
    <td>PICH41264</td>
    <td>pJMLA0.010</td>
    <td>CDS2</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>11</td>
    <td>PAGM1299</td>
    <td>pJMLA0.011</td>
    <td>CDS2 ns</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>12</td>
    <td>PAGM1301</td>
    <td>pJMLA0.012</td>
    <td>CT</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>13</td>
    <td>PICH53388</td>
    <td>pJMLA0.013</td>
    <td>3U</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>14</td>
    <td>PICH41276</td>
    <td>pJMLA0.014</td>
    <td>3U+Ter</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>15</td>
    <td>PICH53399</td>
    <td>pJMLA0.015</td>
    <td>Ter</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>16</td>
    <td>PICH41331</td>
    <td>pJMLA0.016</td>
    <td>L0 Whole</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>17</td>
    <td>PAGM9121</td>
    <td>pJMLA0.017</td>
    <td>Unversal L0 Acceptor</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>18</td>
    <td>L1P1</td>
    <td>pJMLA1.001</td>
    <td>L1P1</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>19</td>
    <td>L1P2</td>
    <td>pJMLA1.002</td>
    <td>L1P2</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>20</td>
    <td>L1P3</td>
    <td>pJMLA1.003</td>
    <td>L1P3</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>21</td>
    <td>L1P4</td>
    <td>pJMLA1.004</td>
    <td>L1P4</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>22</td>
    <td>L1P5</td>
    <td>pJMLA1.005</td>
    <td>L1P5</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>23</td>
    <td>L1P6</td>
    <td>pJMLA1.006</td>
    <td>L1P6</td>
    <td>y</td>
    <td></td>
  </tr>
  <tr>
    <td>24</td>
    <td>L1P7</td>
    <td>pJMLA1.007</td>
    <td>L1P7</td>
    <td>y</td>
    <td></td>
  </tr>
</tbody>
</table>


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
  		alert("Please provide length of backbone acceptor (in bp)");
        document.getElementById("ifYes").style.display = "block";
    	} else {
        document.getElementById("ifYes").style.display = "none";
   		 }
		}
</script>

<script src="http://code.jquery.com/jquery-1.4.2.min.js"></script> <script> var x = document.getElementsByClassName("site-footer-credits"); setTimeout(() => { x[0].remove(); }, 10); </script>



