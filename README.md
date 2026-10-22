# HTQLTTS — Hệ thống quản lý thực tập sinh

Dự án nhóm **TTCS_T926_K10S6_N2**.

## Thành viên
| Họ và tên | Vai trò | Nhánh làm việc |
|---|---|---|
| Phạm Văn Khoa | Trưởng nhóm / Scrum Master | `member/pham-van-khoa` |
| Đinh Bảo Khanh | Frontend | `member/dinh-bao-khanh` |
| Lê Tuấn Hưng | Frontend | `member/le-tuan-hung` |
| Nguyễn Thị Hường | Frontend | `member/nguyen-thi-huong` |
| Nguyễn Hoàng Long | Frontend | `member/nguyen-hoang-long` |
| Hoàng Linh | Backend | `member/hoang-linh` |
| Nguyễn Văn Khánh | Backend | `member/nguyen-van-khanh` |
| Trần Vũ Diệu Linh | Backend | `member/tran-vu-dieu-linh` |

## Chiến lược nhánh
- `main`: nhánh ổn định, chỉ nhận thay đổi đã kiểm tra.
- `dep`: nhánh phát triển chung, tập hợp thay đổi qua Pull Request.
- `member/*`: mỗi thành viên làm việc trên nhánh riêng theo Sprint và nhiệm vụ.
- Luồng tích hợp: `member/*` → Pull Request vào `dep` → kiểm thử, review → Pull Request vào `main`.

## Quy trình Git cho từng thành viên
```bash
git clone https://github.com/ulascutiee-builds/HTQLTTS.git
cd HTQLTTS
git fetch --all
git switch member/ten-thanh-vien
# Sau khi có thay đổi
git add .
git commit -m "feat(sprint1): mo ta nhiem vu"
git push -u origin member/ten-thanh-vien
```

**Lưu ý:** Commit khởi tạo chỉ chứa tài liệu và quy tắc quản lý Git. Mã nguồn từ bản ZIP cần được rà soát và đưa vào nhánh phát triển theo kế hoạch; không đưa file bí mật, cơ sở dữ liệu máy cá nhân hay thư mục build lên repo.
