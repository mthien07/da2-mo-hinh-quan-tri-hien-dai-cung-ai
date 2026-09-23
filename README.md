<p align="center">
  <img src="https://img.shields.io/badge/🐝_HTX_OneBee-AI_Management-8b5cf6?style=for-the-badge&labelColor=0a1628" alt="OneBee AI Management"/>
</p>

<h1 align="center">💼 Mô hình Quản trị Hiện đại cùng AI</h1>

<p align="center">
  <strong>Smart Management — Hệ sinh thái all-in-one cho HTX & SME</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Hội_thi-KNĐMST_2026-f4b942?style=flat-square" alt="Contest"/>
  <img src="https://img.shields.io/badge/Giai_đoạn-Ý_tưởng-00d4aa?style=flat-square" alt="Stage"/>
  <img src="https://img.shields.io/badge/License-MIT-blue?style=flat-square" alt="License"/>
  <img src="https://img.shields.io/badge/HTX_OneBee-MST_1102128064-grey?style=flat-square" alt="Tax ID"/>
</p>

---

## 🎯 Vấn đề

Chuyển đổi số là bài toán sống còn, nhưng hệ thống ERP đóng gói **cồng kềnh** và **tốn kém** (bản quyền theo người dùng, cộng phí tư vấn và tùy biến). Dữ liệu tại nhiều HTX/SME bị **phân mảnh** giữa nhóm chat, Excel và phần mềm kế toán riêng lẻ.

## 💡 Giải pháp

**Lắp ráp thông minh 4 khối quản trị** từ các công cụ SaaS hiện đại kết hợp AI, tạo ra hệ sinh thái all-in-one với phí thiết lập **từ 15 triệu đồng** và lộ trình chuẩn **30 ngày**.

## ✨ Kiến trúc 4 Khối Quản trị

```
┌─────────────────────────────────────────────────────────────┐
│                  🏢 HỆ SINH THÁI ONEBEE                     │
│                                                             │
│  ┌──────────────┐    ┌──────────────┐                       │
│  │  KHỐI 1      │    │  KHỐI 2      │                       │
│  │ 🤝 Vận hành  │    │ 💰 Kế toán   │                       │
│  │ & Cộng tác   │    │ Chuẩn hóa    │                       │
│  │              │    │              │                       │
│  │ LarkSuite    │    │ Misa/KT HTX  │                       │
│  │ Notion       │    │ TT 71/2024   │                       │
│  │ OKRs, Tasks  │    │ Thuế, HĐ     │                       │
│  └──────┬───────┘    └──────┬───────┘                       │
│         │    ┌──────────────┤                                │
│         │    │              │                                │
│  ┌──────▼────▼──────┐                                       │
│  │  KHỐI 3          │    ┌──────────────┐                   │
│  │ ⚡ Tự động hóa   │    │  KHỐI 4      │                   │
│  │                  │    │ 🤖 AI Engine │                   │
│  │ n8n / Hermes     │◄──►│              │                   │
│  │ Zero-touch Ops   │    │ AI Agent     │                   │
│  │ API Gateway      │    │ openclaw     │                   │
│  └──────────────────┘    │ goclaw       │                   │
│                          └──────────────┘                   │
└─────────────────────────────────────────────────────────────┘
```

## 🔑 Tính năng chính

| Khối | Tính năng | Công cụ |
|------|-----------|---------|
| 🤝 **Vận hành** | Quản lý dự án, OKRs, giao tiếp nội bộ, tri thức | LarkSuite / Notion |
| 💰 **Kế toán** | Hóa đơn, thuế, đối soát, báo cáo tài chính | Misa / phần mềm kế toán HTX (Thông tư 71/2024/TT-BTC) |
| ⚡ **Tự động hóa** | API bridge, workflow tự động, zero-touch | n8n / Hermes Agent |
| 🤖 **AI Engine** | Chatbot truy vấn, giám sát, cảnh báo bất thường | openclaw, goclaw, Gemini |

## 🔄 Ví dụ Workflow Tự động

```
📦 Đơn hàng mới trên Shopee
        │
        ▼ (n8n trigger)
┌───────────────────┐
│ Cập nhật Lark     │──► Thông báo team bán hàng
│ Đồng bộ Misa      │──► Ghi nhận doanh thu
│ Kiểm tra tồn kho  │──► Cảnh báo nếu < ngưỡng
│ AI phân tích       │──► Gợi ý bổ sung hàng
└───────────────────┘
```

## 🛠️ Công nghệ sử dụng

| Lớp | Công nghệ |
|-----|-----------|
| Cộng tác | LarkSuite, Notion |
| Kế toán | Misa, phần mềm kế toán HTX |
| Tự động hóa | n8n (self-hosted) |
| AI | Gemini, Ollama, openclaw, goclaw |
| Hạ tầng | Ubuntu Server, Docker |
| Monitoring | Grafana, custom CLI tools |

## 🚀 Chạy Demo

```bash
# Clone repo
git clone https://github.com/mthien07/da2-mo-hinh-quan-tri-hien-dai-cung-ai.git
cd da2-mo-hinh-quan-tri-hien-dai-cung-ai

# Mở demo web (không cần cài đặt)
open demo/index.html
```

> 💡 Demo web **mô phỏng giao diện** Dashboard 4 khối quản trị + AI Chatbot. Dữ liệu minh họa, chưa kết nối n8n/AI thật — dự án đang ở giai đoạn ý tưởng.

## 📁 Cấu trúc dự án

```
da2-mo-hinh-quan-tri-hien-dai-cung-ai/
├── demo/
│   └── index.html          # Web demo Dashboard + AI Chatbot
├── docs/
│   ├── m02-m03-ho-so-du-thi.md  # Hồ sơ dự thi M-02 & M-03
│   ├── pitch-deck.md            # Pitch Deck (10 slides)
│   └── video-script.md          # Kịch bản video 3 phút
└── README.md
```

## 💰 Mô hình kinh doanh

| Nguồn thu | Giá |
|-----------|-----|
| 🔧 Phí Setup ban đầu | 15 - 30 triệu/đơn vị |
| 📆 Phí duy trì/bảo trì hàng tháng | 3 - 5 triệu/tháng |
| 📚 Phí đào tạo bổ sung | 5 triệu/buổi |

## 📌 Trạng thái dự án

- ✅ Hồ sơ dự thi M-02/M-03
- ✅ Pitch Deck
- ✅ Video Script
- ✅ Web Demo tương tác
- 🔄 Triển khai pilot nội bộ (theo kế hoạch 30 ngày)

## 📞 Liên hệ

**Hợp tác xã OneBee**
- 📍 45 đường số 6, KDC Thái Dương, Phường Long An, Tây Ninh
- 📱 0385 944 909
- 🔢 MST: 1102128064
- 👤 Người đại diện: HUỲNH TRỌNG HIẾU

---

<p align="center">
  <em>Dự án dự thi Hội thi Khởi nghiệp Đổi mới Sáng tạo tỉnh Tây Ninh năm 2026</em><br/>
  <strong>🐝 HTX OneBee — Chuyển đổi số cho cộng đồng</strong>
</p>
