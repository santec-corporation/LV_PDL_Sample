# LabVIEW PDL Sample

PDL (Polarization Dependent Loss) test software developed using LabVIEW.

---

## List of content

### Overview of Project

This is an example software of a scan test system for PDL (Polarization Dependent Loss) measurements.

### System Requirements
| Component              | Version/Details       |
|------------------------|------------------------|
| Development Environment | LabVIEW 2017          |
| Instrument DLL          | 2.5.1                 |
| STSProcess.DLL          | 2.2.2                 |
| NI DLL                  | 15.5 or later         |
  
### Tech Stack
  <p align="left"> <a href="https://www.ni.com/ja/shop/labview.html" target="_blank" rel="noreferrer"> <img src="https://th.bing.com/th/id/OIP.YsHSU7SJtV-AHPmwQG72EAHaBS?w=768&h=133&rs=1&pid=ImgDetMain" alt="labview" 
  width="120" height="20"/> </a> </p> 
  
### Configuration
  - TSL Series (TSL-550/TSL-710/TSL-570/TSL-770)
  - MPM Series (MPM-210/210H/211/212/213/215) 
  - PCU Series(PCU-100/PCU-110)
    
***Note: This sample software allows you to control up to two MPM main frames (MPM-210 or MPM-210H)***

### Connection setting
### TSL (Tunable Semiconductor Laser)
  - TSL-550/710: GPIB
  - TSL-570/TSL-770: GPIB, TCP/IP or USB
      
  ***Note: It can be changed on the source code, but the initial value is the delimiter CRLF specification.***
    
### MPM (Multi Port Optical Power meter)
  - MPM-210/210H: GPIB, TCP/IP or USB 

### PCU (Polarization Controller Unit)
  - PCU-100: GPIB 
  - PCU-110: GPIB, TCP/IP or USB

### Line of Reference

#### When Using the **PCU-110**
Use BNC cables to connect the following:

- **TSL - _Trigger Output_** → **MPM - _Trigger Input_**
- **PCU-110 Power Monitor** → **MPM - _Power Monitor_**

<img src="https://github.com/santec-corporation/VS_PDLSample/assets/132535077/a5f5c99a-11cc-44b6-8f12-56e2e3ba67a8" alt="PCU-110 Connection 1" width="500"/>
<br/>
<img src="https://github.com/santec-corporation/VS_PDLSample/assets/132535077/d5cc8e12-63e5-4d01-9a93-f4baa0c4f916" alt="PCU-110 Connection 2" width="500" height="180"/>

#### When Using the **PCU-100**
Use BNC cables to connect the following:

- **TSL - _Trigger Output_** → **PCU-100 _Trigger Input_**
- **PCU-100 _Trigger Output_** → **MPM - _Trigger Input_**

<img src="https://github.com/santec-corporation/VS_PDLSample/assets/132535077/b4276de4-0512-4955-9c2e-aed42e5b8ed5" alt="PCU-100 Connection 1" width="500"/>
<br/>
<img src="https://github.com/santec-corporation/VS_PDLSample/assets/132535077/8177cb72-5abd-4125-9af1-006165323063" alt="PCU-100 Connection 2" width="500"/>


### Operational steps
Refer to the below operational manual to run the script,
  - [ English Manual ](https://github.com/santec-corporation/LV_PDLSample/blob/main/LV_Santec%20PDL%20Swept%20Test%20System%20Manual%20V1.0_EN_20231009.pdf)
  - [ Chinese Manual ](https://github.com/santec-corporation/LV_PDLSample/blob/main/LV_Santec.PDL.Swept.Test.System.Manual.V1.0_CH_20230505.pdf)

---

### For more information on Swept Test System [CLICK HERE](https://inst.santec.com/products/componenttesting/sts)

---