�������� ��� ����� modkam c ������� **FLASH**.

## ��������� 

��� ��������� ������������ ��������� **LED1** (�����).
* ������� � �������� 1 ��, ������������ �������� 500 �� - ����� ������ ��������� ����;
* ���������� �������� - ���������� � ����;
* ��������� ����� �� 1 ���. - ������������� ������� �� ������ **FLASH**;
* ������� � �������� 1 ��, ������������ �������� 100 �� - ����� **Identify**;


## ����������

* ��������� ������� ��������� ������� ������/������������� � ����;
* ��������� ������ **FLASH** ����� 5 ������ �������� � ������ ���������� �� ��������� ���������;
* �������� ������� �� ������ **FLASH** �������� � �������� **ReportAttr** (������� 0x0 Basic, ������� 0x5 modelID);

## Simple Descriptor
```
Endpoint: 1
Profile: Home Automation (0x0104)
Application Device: Unknown (0x0100)
Input Cluster Count: 2
Input Cluster List
    Input Cluster: Basic (0x0000)
    
        Attribute: ZCL Version (0x0000)
        Data Type: 8-Bit Unsigned Integer (0x20)
        Uint8: 1 (0x01)
            
        Attribute: HW Version (0x0003)
        Data Type: 8-Bit Unsigned Integer (0x20)
        Uint8: 1 (0x01)
        
        Attribute: Manufacturer Name (0x0004)
        Data Type: Character String (0x42)
        String: jethome
    
        Attribute: Model Identifier (0x0005)
        Data Type: Character String (0x42)
        String: cc2538.router.v1
   
        Attribute: Date Code (0x0006)
        Data Type: Character String (0x42)
        String: 20200520

    Input Cluster: Identify (0x0003)
Output Cluster Count: 1
Output Cluster List
    Output Cluster: Basic (0x0000)
```