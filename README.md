# POSE Workshop

April 25-27th, 2024

University of Washington 

This repository contains resources for the NSF sponsored Pathways to Open-Source Ecosystems for Laboratory Automation workshop.

To install:

- Clone this repositository recursively: `git clone --recursive https://github.com/machineagency/POSE-workshop.git`
    - Note that the `--recursive` flag is necessary as this repository relies on [science_jubilee](https://github.com/machineagency/science_jubilee/) 
- We recommend using python virtual environments to handle dependencies. To do this:
  - Move into the new directory: `cd POSE-workshop`
  - Create a virtual environment named `.venv`: `python3 -m venv .venv`
  - Activate the virtual environment: `source .venv/bin/activate` 
  - You should now see `(.venv)` to the left of your command line prompt! (If you wish to leave the virtual environment, type `deactivate` from any directory)
- Make sure you're using the latest version of pip: `python3 -m pip install --upgrade pip`
- Install the science_jubilee package: `python3 -m pip install -e ./science_jubilee`
- Add the kernel to jupyter lab: `python3 -m ipykernel install --user --name=POSE-workshop`

## Schedule
_Schedule of 2024.04.18_

<table>
	<thead>
    	<tr>
        	<th> </th>
        	<th>Thursday</th>
        	<th>Friday</th>
        	<th>Saturday</th>
    	</tr>
	</thead>
	<tbody>
    <tr>
      <td>8:30</td>
    	<td rowspan=19>Arrival to Seattle!</td>
    	<td rowspan=2>
		Breakfast/Startup <br>
		in Sieg Building, Room 112 <br>
		<a href="https://maps.app.goo.gl/Hrf4K1v2UZRtQK1q7">3960 Benton Ln NE, Seattle, WA 98195</a>
	</td>
    	<td rowspan=2>
		Breakfast/Startup <br>
		in Sieg Building, Room 112 <br>
		<a href="https://maps.app.goo.gl/Hrf4K1v2UZRtQK1q7">3960 Benton Ln NE, Seattle, WA 98195</a>
	</td>
  	</tr>
  	<tr>
      <td>9:00</td>
  	</tr>
    <tr>
      <td>9:30</td>
    	<td rowspan=2>
		Workshop Intro (<a href="https://github.com/machineagency/POSE-workshop/tree/main/examples">Resources</a>)
	</td>
    	<td rowspan=2>Discussion</td>
  	</tr>
  	<tr>
    	<td>10:00</td>
  	</tr>
    <tr>
      <td>10:30</td>
    	<td>Coffee Break</td>
    	<td>Coffee Break</td>
  	</tr>
  	<tr>
    	<td>11:00</td>
    	<td rowspan=3>Color Matching</td>
    	<td rowspan=3>
		Gel Printing (<a href="https://github.com/machineagency/POSE-workshop/tree/main/gel_printing">Resources</a>) <br>
		&<br>
		Liquid Handling
	</td>
  </tr>
    <tr>
      <td>11:30</td>
  	</tr>
  	<tr>
    	<td>12:00</td>
  	</tr>
    <tr>
      <td>12:30</td>
    	<td rowspan=2>Lunch (provided on-site)</td>
    	<td rowspan=2>Lunch (provided on-site)</td>
  	</tr>
  	<tr>
    	<td>1:00</td>
  	</tr>
    <tr>
      <td>1:30</td>
    	<td rowspan=2>Discussion</td>
    	<td rowspan=2>Discussion</td>
  	</tr>
  	<tr>
    	<td>2:00</td>
  	</tr>
    <tr>
      <td>2:30</td>
    	<td rowspan=5>Tool Assembly & Setup (<a href="https://github.com/machineagency/POSE-workshop/tree/main/tool_setup">Resources</a>)</td>
    	<td rowspan=4>
		Gel Printing (<a href="https://github.com/machineagency/POSE-workshop/tree/main/gel_printing">Resources</a>) <br>
		&<br>
		Liquid Handling
	</td>
  	</tr>
  	<tr>
    	<td>3:00</td>
  	</tr>
    <tr>
      <td>3:30</td>
  	</tr>
  	<tr>
    	<td>4:00</td>
  	</tr>
    <tr>
      <td>4:30</td>
      <td rowspan=3>Discussion and Wrap-up</td>
  </tr>
  	<tr>
    	<td>5:00</td>
    	<td rowspan=2>Discussion</td>
  	</tr>
    <tr>
      <td>5:30</td>
  	</tr>
  	<tr>
    	<td>6:00</td>
    	<td rowspan=6>
		Welcome and happy hour at the <a href=https://escience.washington.edu/>eScience Institute</a><br>
		<a href="https://maps.app.goo.gl/rrRQQeehaGBF83D38">UW Physics/Astronomy Tower, 6th Floor, 3910 15th Ave NE, Seattle, WA 98195 </a>
		</td>
	</td>
    	<td rowspan=6>
		Dinner at Big Time Brewery<br>
		<a href="https://maps.app.goo.gl/V87qcnZR9mzQ3cav6">4133 University Wy NE, Seattle, WA 98105</a>
	</td>
    	<td rowspan=6>
		Dinner at Big Time Brewery<br>
		<a href="https://maps.app.goo.gl/V87qcnZR9mzQ3cav6">4133 University Wy NE, Seattle, WA 98105</a>
	</td>
  	</tr>
    <tr>
      <td>6:30</td>
  	</tr>
  	<tr>
    	<td>7:00</td>
  	</tr>
    <tr>
      <td>7:30</td>
  	</tr>
  	<tr>
    	<td>8:00</td>
  	</tr>
    <tr>
      <td>8:30</td>
  	</tr>
	</tbody>
</table>
