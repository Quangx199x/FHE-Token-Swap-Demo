FHE Token Swap - Complete Setup Guide
📋 Mục lục
1.	Yêu cầu hệ thống
2.	Cài đặt Dependencies
3.	Deploy Smart Contract
4.	Setup Frontend
5.	Sử dụng ứng dụng
________________________________________
🔧 Yêu cầu hệ thống    
•	Node.js >= 18.x    
•	npm hoặc yarn    
•	MetaMask hoặc wallet tương thích    
•	Git
________________________________________
📦 Cài đặt Dependencies
1. Tạo project mới
bash
# Tạo thư mục project
<br>    mkdir fhe-token-swap
cd fhe-token-swap    <br>

# Khởi tạo npm project
npm init -y
2. Cài đặt Hardhat và dependencies cho smart contract
bash
# Cài đặt Hardhat
npm install --save-dev hardhat @nomicfoundation/hardhat-toolbox

# Khởi tạo Hardhat
npx hardhat init
# Chọn: Create a JavaScript project

# Cài đặt fhEVM và dependencies
npm install fhevm @openzeppelin/contracts

# Cài đặt dotenv để quản lý environment variables
npm install --save-dev dotenv
3. Cài đặt Frontend dependencies
bash
# Cài đặt React và Vite
npm create vite@latest frontend -- --template react
cd frontend

# Cài đặt dependencies
npm install

# Cài đặt Zama SDK và ethers
npm install @zama-fhe/relayer-sdk ethers

# Cài đặt UI libraries
npm install lucide-react

# Quay về thư mục root
cd ..
