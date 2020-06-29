���������� ����� 2 ������ (����) � ����� ��������� � 2 ����� (�������� �������, 220 �).
������ ���� � ����� ����� ���� �������� �����. 
| EP | �������� |
| --- | ---- |
| 1 | ���� 1. ���������� ����� ������� �������� onOff (0x0006) |
| 2 | ���� 2. ���������� ����� ������� �������� onOff (0x0006) |
| 3 | ���� 1. ������� Multistate Input 0x0012. �������� 0x17 - ������ ������, 0x16 - ������ �������� |
| 4 | ���� 2. ������� Multistate Input 0x0012. �������� 0x17 - ������ ������, 0x16 - ������ �������� |

�� ��������� ��������� report attributes ��� ��������� onOff (0x0006) � Multistate Input 0x0012.

### ��������� ����� ����� ������� � ����.
����� ������������� �����:
```
    ���� 1 - ���� 1;
    ���� 2 - ���� 2;
```
� �������� OnOff (0x0006) (end point 1, 2) ���������� �������������� �������.

    ID: 0xF000
    Type: uint16 (0x21)
    Value:
        0 - ������ � ���� �� �������;
        1 - ��������� ���� ��������� ��������� ������; (�������� �� ���������)
        2 - ���� ������ ��� ��������� ��� ������� �� ������ (�� ������);
        
        
## ������ ����������
����������� 4 �������� �����.
```
Active Endpoint List
    Endpoint: 1 - ���� 1
    Endpoint: 2 - ���� 2
    Endpoint: 3 - ���� 1
    Endpoint: 4 - ���� 2
```

#### Endpoint: 1
```
Simple Descriptor
    Endpoint: 1
    Profile: Home Automation (0x0104)
    Application Device: Unknown (0x0002)
    Application Version: 0x0001
    Input Cluster Count: 3
        Input Cluster List
            Input Cluster: Basic (0x0000)
                Attribute: ZCL Version (0x0000)
                Uint8: 2 (0x02)
                Attribute: HW Version (0x0003)
                Uint8: 1 (0x01)
                Attribute: Manufacturer Name (0x0004)
                String: JETHOME
                Attribute: Model Identifier (0x0005)
                String: jethome.double_relay.v2
                Attribute: Date Code (0x0006)
                String: May 14 2020 
            Input Cluster: Identify (0x0003)
            Input Cluster: On/Off (0x0006)
    Output Cluster Count: 1
        Output Cluster List
            Output Cluster: OTA Upgrade (0x0019)
```
#### Endpoint: 2
```
Simple Descriptor
    Endpoint: 2
    Profile: Home Automation (0x0104)
    Application Device: Unknown (0x0002)
    Application Version: 0x0001
    Input Cluster Count: 2
        Input Cluster List
            Input Cluster: On/Off (0x0006)
            Input Cluster: Basic (0x0000)
    Output Cluster Count: 0
```
#### Endpoint: 3
```
Simple Descriptor
    Endpoint: 3
    Profile: Home Automation (0x0104)
    Application Device: Unknown (0x0002)
    Application Version: 0x0001
    Input Cluster Count: 2
        Input Cluster List
            Input Cluster: Multistate Input (Basic) (0x0012)
            Input Cluster: Basic (0x0000)
    Output Cluster Count: 0
```
#### Endpoint: 4
```
Simple Descriptor
    Endpoint: 4
    Profile: Home Automation (0x0104)
    Application Device: Unknown (0x0002)
    Application Version: 0x0001
    Input Cluster Count: 2
        Input Cluster List
            Input Cluster: Multistate Input (Basic) (0x0012)
            Input Cluster: Basic (0x0000)
    Output Cluster Count: 0
```