## Dataset

The following dataset was used in the paper submitted to Sensors MDPI: Monitoring System for Online Fault Detection and Classification in Photovoltaic Plants by André E. Lazzaretti, Clayton H. da Costa, Marcelo P. Rodrigues, Guilherme D.Yamada, Gilberto Lexinoski, Guilherme L. Moritz, Elder Oroski, Rafael E. de Góes, Robson R. Linhares, Paulo C. Stadzisz, Júlio S. Omori, and Rodrigo B. dos Santos.

## Photovoltaic fault dataset

This dataset contains 16 days of data of a grid-tie photovoltaic plant's operation with both faulty and normal operation. The dataset is divided into 2 '.mat' files (which can be loaded with MATLAB). 

## Photovoltaic plant's description

The photovoltaic plant used to collect this data has 2 strings with 8x C6SU-330P PV Modules each. Both strings are connected to a 5kW gridtie power inverter (NHS Solar 5K-GDM1).
## Files description:
  
  * 1 - dataset_elec.mat -> DC Electrical data (Voltage and Current of both strings)
  
  * 2 - dataset_amb.mat -> Temperature, Irradiance and Fault class label

## Variables description:

  <table>
    <thead>
      <th>Variable</th>
      <th>Description</th>
    </thead>
    <tbody>
      <tr>
        <td>vdc1</td>
        <td>Voltage - String 1</td>
      </tr>
      <tr>
        <td>vdc2</td>
        <td>Voltage - String 2</td>
      </tr>  
      <td>idc1</td>
        <td>Current - String 1</td>
      </tr>     
      <td>idc2</td>
        <td>Current - String 2</td>
      </tr>
        <td>irr</td>
        <td>Irradiance</td>
      </tr>
      <td>pvt</td>
        <td>PV Module Temperature</td>
      </tr>
      <td>f_nv</td>
        <td>Fault Label</td>
      </tr>
  </tbody>
</table>
      
## Fault label (f_nv)
  <table>
    <thead>
      <th>Value</th>
      <th>Description</th>
    </thead>
    <tbody>
      <tr>
        <td>0</td>
        <td>Normal Operation (No faults)</td>
      </tr>
      <tr>
        <td>1</td>
        <td>Short-Circuit (Short Circuit between 2 modules of a String)</td>
      </tr>
       <tr>
        <td>2</td>
        <td>Degradation (There is a resistance between 2 modules of a String)</td>
      </tr>     
      <tr>
        <td>3</td>
        <td>Open Circuit (One String disconnected from the power inverter)</td>
      </tr>
      <tr>
        <td>4</td>
        <td>Shadowing (Shadow in one or more modules)</td>
      </tr> 
    </tbody>     
</table>

## The Faults

Degradation, Short-Circuit and Open Circuit are artificially introduced, while the shadowing is natural (shade produced by nearby buildings).

Degradation was introduced via a resistive load bank between two modules.

Short-Circuit was introduced with a cable connected between the positive connection of a module and the negative connection of the adjacent module.

Open Circuit was introduced with the oppening of one string's main circuit breaker.
      
