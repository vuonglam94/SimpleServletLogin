# Simple Servlet Login

## Environment

- JDK8
- TOMCAT8

Ứng dụng gồm 2 Role là **EMPLOYEE** và **MANAGER**:

1. Vai trò **EMPLOYEE** cho phép truy cập 2 trang */userInfo* và */employeeTask*
2. Vai trò **MANAGER** cho phép truy cập 2 trang */userInfo* và */managerTask*

Các trang khác trong ứng dụng ko yêu cầu đăng nhập

Có 2 User là **employee1** và **manager1**

1. User **employee1** có Role **EMPLOYEE**
2. User **manager1** có Role **EMPLOYEE** và **MANAGER**

Nếu User chưa đăng nhập sẽ redirect về trang */login*

Nếu User đã đăng nhập và truy cập vào trang ko được phép theo Role sẽ hiển thị thông báo **Access Denied**