<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th colspan="2"><blockquote>
<p>ESCP-BMS1 Evaluation Software Manual</p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><blockquote>
<p>Title</p>
</blockquote></td>
<td><blockquote>
<p>ESCP-BMS1 Evaluation Software Manual</p>
</blockquote></td>
</tr>
<tr class="even">
<td><blockquote>
<p>Doc Ref</p>
</blockquote></td>
<td><blockquote>
<p>ESS-243/080120/EXC-REV.01</p>
</blockquote></td>
</tr>
</tbody>
</table>

<img src="./media/f1.jpg"
style="width:2.97829in;height:2.09458in" />

> DOCUMENT TRACKING TABLE

<table>
<colgroup>
<col style="width: 18%" />
<col style="width: 18%" />
<col style="width: 63%" />
</colgroup>
<thead>
<tr class="header">
<th><blockquote>
<p>Version</p>
</blockquote></th>
<th><blockquote>
<p>Date</p>
</blockquote></th>
<th><blockquote>
<p>Reason for change</p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><blockquote>
<p>1</p>
</blockquote></td>
<td></td>
<td><blockquote>
<p>Initial version</p>
</blockquote></td>
</tr>
</tbody>
</table>

1.  Data Readout GUI

    1.  # Software Installation

> To install the Pressure Sensor Evaluation Software:

- Extract the contents of the PSES.zip file and navigate to the “Volume”
  folder.

- Run setup.exe (as administrator if possible) and follow the
  installation wizard.

- Once the installation is complete run PSES.exe

  1.  # Application Description



<img src="./media/f2.jpg"
style="width:7.61346in;height:7.48648in" />

<table>
<colgroup>
<col style="width: 8%" />
<col style="width: 91%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>#</strong></th>
<th><blockquote>
<p><strong>Description</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1</td>
<td><blockquote>
<p>Connection row</p>
</blockquote></td>
</tr>
<tr class="even">
<td>2</td>
<td><blockquote>
<p>Device scan</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>3</td>
<td><blockquote>
<p>Data display</p>
</blockquote></td>
</tr>
<tr class="even">
<td>4</td>
<td><blockquote>
<p>Open data graph window</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>5</td>
<td><blockquote>
<p>Log file configuration</p>
</blockquote></td>
</tr>
<tr class="even">
<td>6</td>
<td><blockquote>
<p>Evaluation Software version</p>
</blockquote></td>
</tr>
</tbody>
</table>

1.  **Connection Row**

> Use the *Serial Port* dropdown box to select the COM port that
> corresponds to the Evaluation Kit and press the *Connect* button,
> which upon successful connection will change color and its text will
> now display *Disconnect*. Pressing *Disconnect* will stop
> communication with the Evaluation Kit. After connection with the kit
> is established the software will automatically scan for connected
> devices (see Device Scan below). This can take a few seconds.

2.  **Device Scan**

> The software scans for connected devices and displays the results in a
> table. The table columns indicate the channel number, an LED that goes
> green when a device is connected to the channel, the device’s serial
> number and the device’s I<sup>2</sup>C slave address (in hex). Device
> scan is performed automatically after successfully establishing a
> connection with the Evaluation Kit or can be manually started by
> pressing the *Scan Devices* button. The scan progress is indicated by
> a progress bar below the button. If a device is found on any channel
> the *Devices Connected* LED lights green.

3.  **Data display**

> The received data values are displayed in this table, both the
> floating-point value for each measured quantity and the raw 16-bit
> hexadecimal value. The user can choose which device’s data is
> displayed by selecting the appropriate channel. The user can also
> choose the sample rate of the data. The minimum sample rate is 1ms.
> The same sample rate applies to the graphs and the *Log File*. The
> user can pause data acquisition at any time by pressing the *Stop Data
> Acquisition* button.

4.  **Open data graph window**

> Pressing the button will open the *Graph Window*

><img src="./media/f3.jpg"
style="width:7.61346in;height:6.48648in" />

> Using the drop-down menu (1) the user can select the quantity to
> display. By default, data for all connected sensors is displayed but
> the user can select/deselect any of them (2). The user can also
> zoom/pan the graph area using the respective buttons (3) and clear the
> graph area by pressing the *Clear History* button (4).

5.  **Log File Configuration**

> Optionally the user can log the received data to a file. Use the
> *Browse* button (folder icon) to select a directory and name for the
> log file and press the button to start logging. Pressing the button
> again

> will stop logging. Data is logged to the file at the rate specified in
> the Sample Rate textbox as tab delimited values. Measured quantities
> are written in the following order

<table>
<colgroup>
<col style="width: 42%" />
<col style="width: 57%" />
</colgroup>
<thead>
<tr class="header">
<th><blockquote>
<p><strong>Pressure</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Temperature</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

> For each measured quantity we log its floating-point value with 6
> digits of precision. An example is shown below:

><img src="./media/f4.jpg"
style="width:7.61346in;height:4.48648in" />

> **Figure 4: Data File format**
>
> A log file for each serial number will be created storing the
> corresponding data.

6.  **Evaluation Software Version**

> Displays the current version of the application
