# BÀI LÀM – HACKATHON 01

- **Mã đề:** 20
- **Họ tên:**Phạm Thành Đạo 
- **Lớp:**HCM-KS26-CNTT1 
- **Link repository:** 
- **Hệ điều hành (Windows/macOS):** macOS

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```
cd /Users/phamdao/Documents
pwd
mkdir -p salon-toc-website/{docs,media,data,logs,backup}
ls -aR

```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```.        .DS_Store    data        logs
..        backup        docs        media

./backup:
.            ..            logo_salon_toc.png

./data:
.                ..                hoa_don_salon_thang_11.xlsx

./docs:
.            ..            lich_lam_viec.txt

./logs:
.            ..            daily_report.txt    salon.log

./media:
.            ..            logo_salon_toc.png
phamdao@MacBook-Pro-cua-Pham salon-toc-website %

```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
#   cd /Users/phamdao/Documents/salon-toc-website/logs grep -p 'ERROR' /Users/phamdao/Documents/salon-toc-website/logs/salon.log   > /Users/phamdao/Documents/salon-toc-website/logs/daily_report.txt

```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```
2026-11-28 09:53:35 [ERROR] Khong tim thay trang /kieu-toc-moi (404)
2026-11-28 09:57:35 [ERROR] Khong tim thay trang /kieu-toc-moi (404)
```

## 4.4. Thao tác với tài liệu Markdown (README.md)

> README.md được chấm trực tiếp trên file `README.md` ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [x] Heading 1: tên dự án
- [x] Mô tả ngắn có cả **in đậm** và *in nghiêng*
- [x] Bảng `Thư mục | Nội dung`, ít nhất 3 dòng dữ liệu
- [x] Code block chứa lệnh PowerShell/Terminal liệt kê nội dung dự án
- [x] Task list ít nhất 2 công việc, có ít nhất 1 mục đã hoàn thành
- [x] Blockquote nhắc không upload `.env`

## 4.5. Chạy script auto_report (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
grep -p 'ERROR' /Users/phamdao/Documents/salon-toc-website/logs/salon.log   > /Users/phamdao/Documents/salon-toc-website/logs/daily_report.txt

```

### Kết quả hiển thị

```echo"==================================================
       === TONG HOP LOG ===
       Ngay gio: 28/10/2026 08:43
==================================================


--------------------------------------------------
CAC DONG CHUA WARNING:4
SO DONG CHUA ERROR:5"

```

## 4.6. Đếm số dòng lỗi

### Lệnh

```shell


```

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

```text
5

```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
# echo "       === TONG HOP LOG ==="

 echo "       Ngay gio: $(date '+%d/%m/%Y %H:%M')"

 echo "=================================================="

 echo ""

 grep -p 'ERROR' /Users/phamdao/Documents/salon-toc-website/logs/salon.log   > /Users/phamdao/Documents/salon-toc-website/logs/daily_report.txt

```

### Nội dung file logs/tong_hop.txt

```text
==================================================
       === TONG HOP LOG ===
       Ngay gio: 28/10/2026 08:43
==================================================


--------------------------------------------------
CAC DONG CHUA WARNING:4
SO DONG CHUA ERROR:5

```

## 4.8. Excel

> Phần Excel được chấm trực tiếp trên file `data/hoa_don_salon_thang_11.xlsx`, không cần ghi vào đây.
