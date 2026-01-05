# Hồ Ngọc Phương - Website Cá Nhân

Đây là website cá nhân được xây dựng bằng Docusaurus và được triển khai trên GitHub Pages.

## 📋 Yêu cầu hệ thống

Để chạy website này trên máy của bạn, bạn cần một trong các phương pháp sau:

- **Python 3** (có sẵn trên hầu hết các hệ điều hành)
- **Node.js** và npm (khuyến nghị cho phát triển web)
- Hoặc bất kỳ web server nào khác (Apache, Nginx, etc.)

## 🚀 Cách chạy website trên máy local

### Phương pháp 1: Sử dụng Python (Đơn giản nhất)

Python thường được cài đặt sẵn trên macOS và Linux. Trên Windows, bạn có thể tải từ [python.org](https://www.python.org/downloads/).

#### Python 3:
```bash
# Di chuyển vào thư mục dự án
cd hongocphuong.github.io

# Chạy web server
python3 -m http.server 8000

# Hoặc trên Windows:
python -m http.server 8000
```

Sau đó mở trình duyệt và truy cập: **http://localhost:8000**

### Phương pháp 2: Sử dụng Node.js và npx

Nếu bạn đã cài đặt Node.js, bạn có thể sử dụng các package sau:

#### Sử dụng serve (Khuyến nghị):
```bash
# Di chuyển vào thư mục dự án
cd hongocphuong.github.io

# Chạy với npx (không cần cài đặt)
npx serve

# Hoặc cài đặt globally:
npm install -g serve
serve
```

#### Sử dụng http-server:
```bash
# Di chuyển vào thư mục dự án
cd hongocphuong.github.io

# Chạy với npx
npx http-server

# Hoặc cài đặt globally:
npm install -g http-server
http-server
```

Sau đó mở trình duyệt và truy cập địa chỉ được hiển thị (thường là http://localhost:3000 hoặc http://localhost:8080)

### Phương pháp 3: Sử dụng PHP

Nếu bạn có PHP đã cài đặt:

```bash
# Di chuyển vào thư mục dự án
cd hongocphuong.github.io

# Chạy PHP development server
php -S localhost:8000
```

Sau đó mở trình duyệt và truy cập: **http://localhost:8000**

### Phương pháp 4: Sử dụng Live Server (VS Code Extension)

Nếu bạn sử dụng Visual Studio Code:

1. Cài đặt extension "Live Server" từ Ritwick Dey
2. Mở thư mục dự án trong VS Code
3. Click chuột phải vào file `index.html`
4. Chọn "Open with Live Server"

## 📁 Cấu trúc dự án

```
hongocphuong.github.io/
├── index.html          # Trang chủ
├── blog.html           # Trang blog
├── search.html         # Trang tìm kiếm
├── 404.html            # Trang lỗi 404
├── assets/             # Thư mục chứa CSS, JS, và hình ảnh
│   ├── css/            # Stylesheet files
│   ├── js/             # JavaScript files
│   └── images/         # Hình ảnh
├── blog/               # Các bài viết blog
├── docs/               # Tài liệu
├── img/                # Hình ảnh chung
├── vi/                 # Nội dung tiếng Việt
└── .nojekyll           # File cấu hình GitHub Pages
```

## 🛠️ Về Docusaurus

Website này được build từ Docusaurus - một framework tạo trang tài liệu tĩnh của Facebook/Meta. Đây là version đã được build sẵn (static HTML/CSS/JS), sẵn sàng để triển khai.

### Nếu bạn muốn chỉnh sửa và rebuild website:

Bạn cần tìm source code gốc (thường nằm ở một branch khác hoặc repository khác) có chứa:
- `package.json`
- `docusaurus.config.js`
- Thư mục `docs/`, `blog/`, `src/`

Sau đó chạy các lệnh:
```bash
npm install           # Cài đặt dependencies
npm run start         # Chạy development server
npm run build         # Build static files
```

## 📝 Lưu ý

- Đây là một website tĩnh (static site), không yêu cầu database hay backend server
- Tất cả nội dung đã được build sẵn và có thể chạy trực tiếp
- Website này đang được host trên GitHub Pages tại: https://hongocphuong.github.io

## 🔗 Links hữu ích

- [Docusaurus Documentation](https://docusaurus.io/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

## ❓ Câu hỏi thường gặp

**Q: Tôi có cần cài đặt Docusaurus không?**
A: Không, website này đã được build sẵn. Bạn chỉ cần một web server đơn giản để chạy các file HTML.

**Q: Tại sao tôi thấy lỗi 404 khi chuyển trang?**
A: Hãy đảm bảo bạn đang chạy web server từ thư mục gốc của dự án (nơi chứa file `index.html`).

**Q: Làm sao để chỉnh sửa nội dung website?**
A: Để chỉnh sửa nội dung, bạn cần source code gốc của Docusaurus. Repository này chỉ chứa bản build sẵn.

**Q: Port 8000 đã được sử dụng, làm sao đổi port?**
A: Thay đổi số port trong lệnh, ví dụ: `python3 -m http.server 3000`

## 📧 Liên hệ

Nếu có bất kỳ câu hỏi nào, vui lòng tạo issue trên GitHub repository này.
