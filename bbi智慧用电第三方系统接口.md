> ���ĵ�����POST����ʽ���䣬JSON���ݸ�ʽ��UTF-8����.

>�����������ͷ�Ϊ2���������ݣ�1�ָ澯����

>��HTTP״̬��200�ж��Ƿ����ͳɹ������ɹ����ݲ������Ϊ10���ӡ�20���ӡ�30���ӡ�

# ��1����������֡1
���� | ���� | �Ƿ���� | ���� | ʾ��ֵ
-|-|-|-|-
meterNo | String | �� | ���
sjsj | String | �� | ����ʱ��
axdy | number | �� |A���ѹ(V)
bxdy | number | �� |B���ѹ(V)
cxdy | number | �� |C���ѹ(V)
axdl | number | �� |A�����(A)
bxdl | number | �� |B�����(A)
cxdl | number | �� |C�����(A)
sydl | number | �� |ʣ�����(A)
zyggl | number | �� |���й�����(kW)
zglys | number | �� |�ܹ�������
zxygzdl | number | �� |�����й��ܵ���(kWh)

> ����ʾ����
    
    {
        "meterNo" : "111800000490",
        "sjsj" : "2019-04-16 16:00:00",
        "data" : {
                "axdy" : 220,
                "bxdy" : 220,
                "bxdy" : 220,
                 ...
                 // ������1�������...
                }
    }

# ��2����������֡2
���� | ���� | �Ƿ���� | ���� | ʾ��ֵ
-|-|-|-|-
meterNo | String | �� | ���
sjsj | String | �� | ����ʱ��
axwd | number | �� |A���¶�(��)
bxwd | number | �� |B���¶�(��)
cxwd | number | �� |C���¶�(��)
lxwd | number | �� |�����¶�(��)
hjwd | number | �� |�����¶�(��)

> ����ʾ����
    
    {
        "meterNo" : "111800000490",
        "sjsj" : "2019-04-16 16:00:00",
        "data" : {
                "axwd" : 20,
                "axwd" : 20,
                "axwd" : 20,
                 ...
                 // ������2�������...
                }
    }
    
# ��4���澯���� ����
���� | ���� | �Ƿ���� | ���� | ʾ��ֵ
-|-|-|-|-
meterNo | String | �� | ���
sjsj | String | �� | ����ʱ��
code | String | �� |�澯���� 
data | Json | �� |���ָ澯������ֵ�ǰֵ

## data����
���� | ���� | �Ƿ���� | ���� | ʾ��ֵ
-|-|-|-|-
axdy | number | �� |A���ѹ(V)
bxdy | number | �� |B���ѹ(V)
cxdy | number | �� |C���ѹ(V)
axdl | number | �� |A�����(A)
bxdl | number | �� |B�����(A)
cxdl | number | �� |C�����(A)
sydl | number | �� |ʣ�����(A)
zyggl | number | �� |���й�����(kW)
zglys | number | �� |�ܹ�������
axwd | number | �� |A���¶�(��)
bxwd | number | �� |B���¶�(��)
cxwd | number | �� |C���¶�(��)
lxwd | number | �� |�����¶�(��)
hjwd | number | �� |�����¶�(��)

> ����ʾ����
    
    {
        "meterNo" : "111800000490",
        "sjsj" : "2019-04-16 16:00:00",
        "code" : "10001",
        "data" : {
                "axdy" : 600,
                "bxdy" : 100,
                "cxdy" : 200,
                 ...
                 // ����data�����������...
                }
    }
##�澯code����
> ���ݺ�������

|code|�¼�|
|-|-|
|....|....|
|....|....      