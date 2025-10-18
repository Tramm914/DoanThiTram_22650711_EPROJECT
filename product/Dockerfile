# Sử dụng Node.js base image
FROM node:18

# Tạo thư mục làm việc
WORKDIR /app

# Sao chép package.json và cài dependencies
COPY package*.json ./
RUN npm install

# Sao chép toàn bộ mã nguồn
COPY . .

# Expose port tương ứng (sẽ lấy từ .env)
EXPOSE 3001

# Lệnh chạy app
CMD ["npm", "start"]
