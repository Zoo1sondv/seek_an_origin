
## Installation and Setup
Prerequisites : `npm, git, docker(optional)`

**Bước 1:**
Clone the repository và sau đó cd vào thư mục vừa clone về
```Bash
git clone https://github.com/Zoo1sondv/seek_an_origin.git
cd seek_an_origin
```

**Bước 2:**
Tại thư mục seek_an_origin:
- Cài đặt các gói dependence npm
```Bash 
npm i 
```
- Cài đặt ganache-cli
```Bash
npm i -g ganache-cli
```
- Cài đặt truffle
```Bash
npm install -g truffle
```

- Migrate the contracts
```Bash
truffle migrate --network=develop --reset
truffle migrate
```

Configure ganache-cli for 10 accounts and extend gasLimit to 6721975000 and beyond, so as to have enough gas for migrating the smart contracts and a data flow for the prototype.  
```Bash
ganache-cli --accounts 10 --gasLimit 6721975000
```

**Bước 3:**
Truy cập vào thư mục client
```Bash
cd /seek_an_origin/client
```

Tại thư mục client:
- Cài đặt các gói dependence npm
Install all packages in the package.json file
```Bash
npm i
```




**Bước 4:**
- Cài đặt các phần mềm liên quan: Đọc file setup.docx
- Thay đổi giá trị REACT_APP_ADDRESS_INIT trong .env bằng địa chỉ address index 0 trong ganache

**Bước 5:**
- Chạy ứng dụng web tại cổng 3000
```Bash
npm start
```

- Ta có thể tiến hành quá trình tương tác với website.


**LƯU Ý**
Mỗi khi thay đổi giá trị trong file .env thì cần stop và npm start lại

