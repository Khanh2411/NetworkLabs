# OSPF (Multi-area)
## Mô tả tổng quan sơ đồ
![Topology](images/Topology.png)
Đây là mạng WAN mô phỏng với OSPF multi-area, có 4 router chính (R1, R2, R3, R4) kết nối với nhau, kèm theo các máy PC (VPC7, VPC8, VPC9).  
Mạng được chia thành các area trong OSPF:  
- Area 0 (Backbone area): kết nối giữa R1 và R4.  
- Area 1: kết nối giữa R2 ↔ R4.  
- Area 2: kết nối giữa R3 ↔ R4.

R4 với vai trò là Core Router / ABR (Area Border Router):  
- Trung tâm mạng WAN, kết nối giữa backbone Area 0 và các area khác.  
- Làm ABR: kết nối nhiều area trong OSPF.

## Cấu hình OSPF (Multi-area)
Đặt IP cho từng router:
R1:  
![Topology](images/setipR1.png)  
R2:  
![Topology](images/setipR2.png)  
R3:  
![Topology](images/setipR3.png)   
R4:  
![Topology](images/setipR4.png)  
  
Cấu hình OSPF:  
R1:  
![Topology](images/ospfR1.png)  
R2:  
![Topology](images/ospfR2.png)  
R3:  
![Topology](images/ospfR3.png)  
R4:  
![Topology](images/ospfR4.png)  
  
Kết nối internet cho các area khác.  
![Topology](images/accesinternet.png)  

Kiểm tra neighbor:  
    
Kiểm tra kết nối:  
VPC7:  
![Topology](images/testconnect1.png)  
VPC8:  
![Topology](images/testconnect2.png)  

