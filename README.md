# Student Score Regression

Ứng dụng hồi quy tuyến tính (scikit-learn) với giao diện ipywidgets, chạy bằng Voilà và triển khai trên Render.

> Dữ liệu là dữ liệu tổng hợp phục vụ giảng dạy. Không dùng mô hình này để đánh giá sinh viên thật.

## Chạy cục bộ

```bash
python -m venv .venv
# Windows PowerShell: .venv\Scripts\Activate.ps1
# Linux/macOS:        source .venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt

python -m training.generate_data
python -m training.train_model
voila app.ipynb --no-browser --port=8866
```

Mở http://localhost:8866

## Triển khai

Commit `artifacts/linear_regression.joblib`, đẩy lên GitHub, tạo Blueprint trên Render từ `render.yaml`.
