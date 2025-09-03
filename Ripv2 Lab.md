# RIP Routing
RIP là một giao thức định tuyến động (dynamic routing protocol) thuộc distance-vector routing.  
Nó cho phép các router trao đổi thông tin bảng định tuyến với nhau, để tự động học được đường đi đến các mạng khác mà không cần cấu hình static route thủ công.  

## Đặc điểm chính của RIP
- Thuộc loại: Distance-vector (dựa vào số hop count để chọn đường đi).
- Metric: Số hop (mỗi router đi qua tính là 1 hop).
- Giới hạn: Tối đa 15 hop, nếu xa hơn coi như không reach.
- Cập nhật: Định kỳ gửi toàn bộ bảng định tuyến cho láng giềng sau mỗi 30 giây (broadcast/multicast).
- Dễ cấu hình nhưng không tối ưu cho mạng lớn do giới hạn hop và tốc độ hội tụ chậm.

## Sơ đồ mạng RIP
![](images/TopologyRIP.png)  
  
## Cấu hình RIPv2
### Cấu hình IP
#### R1
![](images/RIP_IPR1.png)  
#### R2
![](images/RIP_IPR2.png)  
#### R3
![](images/RIP_IPR3.png)  
  
### Cấu hình RIPv2
#### R1
![](images/RIP_R1.png)  
#### R2
![](images/RIP_R2.png)  
#### R3
![](images/RIP_R3.png)  
  
### Kiểm tra cấu hình RIPv2
#### R1
![](images/ShowRIPconf1.png)  
#### R2
![](images/ShowRIPconf2.png)  
#### R3
![](images/ShowRIPconf3.png)  
  
### Kiểm tra kết nối
#### VPC1
![](images/RIP_Conncection1.png)  
#### VPC2
![](images/RIP_Conncection2.png)  
#### VPC3
![](images/RIP_Conncection3.png)  
  
